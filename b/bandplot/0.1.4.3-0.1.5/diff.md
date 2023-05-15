# Comparing `tmp/bandplot-0.1.4.3-py3-none-any.whl.zip` & `tmp/bandplot-0.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,12 @@
-Zip file size: 10214 bytes, number of entries: 9
--rw-rw-r--  2.0 unx       26 b- defN 23-May-12 23:05 bandplot/__init__.py
--rw-rw-r--  2.0 unx    32523 b- defN 23-May-12 23:05 bandplot/plots.py
--rw-rw-r--  2.0 unx     6111 b- defN 23-May-12 23:05 bandplot/readdata.py
--rw-rw-r--  2.0 unx    16829 b- defN 23-May-12 23:05 bandplot/wrapper.py
--rw-rw-r--  2.0 unx     2954 b- defN 23-May-12 23:05 bandplot-0.1.4.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-12 23:05 bandplot-0.1.4.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx       86 b- defN 23-May-12 23:05 bandplot-0.1.4.3.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        9 b- defN 23-May-12 23:05 bandplot-0.1.4.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      711 b- defN 23-May-12 23:05 bandplot-0.1.4.3.dist-info/RECORD
-9 files, 59341 bytes uncompressed, 8990 bytes compressed:  84.9%
+Zip file size: 13124 bytes, number of entries: 10
+-rw-rw-r--  2.0 unx       24 b- defN 23-May-15 02:20 bandplot/__init__.py
+-rw-rw-r--  2.0 unx     6896 b- defN 23-May-15 02:20 bandplot/mass.py
+-rw-rw-r--  2.0 unx    36761 b- defN 23-May-15 02:20 bandplot/plots.py
+-rw-rw-r--  2.0 unx     6111 b- defN 23-May-15 02:20 bandplot/readdata.py
+-rw-rw-r--  2.0 unx    20407 b- defN 23-May-15 02:20 bandplot/wrapper.py
+-rw-rw-r--  2.0 unx     2951 b- defN 23-May-15 02:20 bandplot-0.1.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-15 02:20 bandplot-0.1.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       86 b- defN 23-May-15 02:20 bandplot-0.1.5.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        9 b- defN 23-May-15 02:20 bandplot-0.1.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      774 b- defN 23-May-15 02:20 bandplot-0.1.5.dist-info/RECORD
+10 files, 74111 bytes uncompressed, 11812 bytes compressed:  84.1%
```

## zipnote {}

```diff
@@ -1,28 +1,31 @@
 Filename: bandplot/__init__.py
 Comment: 
 
+Filename: bandplot/mass.py
+Comment: 
+
 Filename: bandplot/plots.py
 Comment: 
 
 Filename: bandplot/readdata.py
 Comment: 
 
 Filename: bandplot/wrapper.py
 Comment: 
 
-Filename: bandplot-0.1.4.3.dist-info/METADATA
+Filename: bandplot-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: bandplot-0.1.4.3.dist-info/WHEEL
+Filename: bandplot-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: bandplot-0.1.4.3.dist-info/entry_points.txt
+Filename: bandplot-0.1.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: bandplot-0.1.4.3.dist-info/top_level.txt
+Filename: bandplot-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: bandplot-0.1.4.3.dist-info/RECORD
+Filename: bandplot-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bandplot/__init__.py

```diff
@@ -1,3 +1,3 @@
 
-__version__ = "0.1.4.3"
+__version__ = "0.1.5"
```

## bandplot/plots.py

```diff
@@ -18,15 +18,15 @@
     plt.legend(legend, frameon=False, prop={'size':'medium'}, loc=fig_p.location)
     plt.xlim(arr[0], arr[-1])
     plt.ylim(fig_p.vertical)
     plt.ylabel('Energy (eV)')
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
 def Noneispin2(arr, bands, ticks, labels, legend, fig_p):
-    fig = plt.figure(figsize=fig_p.size)
+    plt.figure(figsize=fig_p.size)
     color = fig_p.color or ['r', 'k']
     linestyle = fig_p.linestyle or ['-', '-.']
     linewidth = fig_p.linewidth or [0.8, 0.8]
     if len(color) == 1:
         color = [color[0], 'k']
     if len(linestyle) == 1:
         linestyle = [linestyle[0], '-.']
@@ -128,16 +128,16 @@
     linewidth = fig_p.linewidth or [0.8, 0.8, 0.8, 0.8]
     if len(color) < 4:
         color = color + [''] * (4 - len(color))
     if len(linestyle) < 4:
         linestyle = linestyle + ['-'] * (4 - len(linestyle))
     if len(linewidth) < 4:
         linewidth = linewidth + [0.8] * (4 - len(linewidth))
-    f1 = ax1.plot(arr[0], bands[0][0].T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0], label='1')
-    f2 = ax2.plot(arr[0], bands[0][1].T, color=color[1], linewidth=linewidth[1], linestyle=linestyle[1], label='1')
+    f1 = ax1.plot(arr[0], bands[0][0].T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
+    f2 = ax2.plot(arr[0], bands[0][1].T, color=color[1], linewidth=linewidth[1], linestyle=linestyle[1])
     L = ax1.legend([], frameon=False, loc='lower left', title=legend[0], title_fontproperties={'size':'medium'})
     ax1.add_artist(L)
     ax1.tick_params(axis='y', which='minor', color='gray')
     ax2.tick_params(axis='y', which='minor', color='gray')
 
     ax1.axhline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.axhline(linewidth=0.4, linestyle='-.', c='gray')
@@ -160,23 +160,23 @@
     ax1.set_ylabel('Energy (eV)')
     ax1_f = fig.add_subplot(1,2,1)
     g1 = ax1_f.plot(arr[1], bands[1][0].T, color=color[2], linewidth=linewidth[2], linestyle=linestyle[2])
     ax1_f.set_xlim(arr[1][0], arr[1][-1])
     ax1_f.set_ylim(fig_p.vertical)
     ax1_f.axis('off')
     ax2_f = fig.add_subplot(1,2,2)
-    g2 = ax2_f.plot(arr[1], bands[1][1].T, color=color[3], linewidth=linewidth[3], linestyle=linestyle[3], label='2')
+    g2 = ax2_f.plot(arr[1], bands[1][1].T, color=color[3], linewidth=linewidth[3], linestyle=linestyle[3])
     ax2_f.set_xlim(arr[1][0], arr[1][-1])
     ax2_f.set_ylim(fig_p.vertical)
     ax2_f.axis('off')
     ax1.legend([f1[0], g1[0]], [legend[1], legend[2]], frameon=False, prop={'size':'medium'}, loc=fig_p.location, alignment='left', title='up', title_fontproperties={'style':'italic', 'size':'medium'})
     ax2.legend([f2[0], g2[0]], [legend[1], legend[2]], frameon=False, prop={'size':'medium'}, loc=fig_p.location, alignment='left', title='down', title_fontproperties={'style':'italic', 'size':'medium'})
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
-def NoneispinWd(arr, bands, ticks, labels, darr, dele, fill, index_f, elements, width_ratios, legend, fig_p):
+def NoneispinWd(arr, bands, ticks, labels, darr, dele, index_f, elements, width_ratios, legend, fig_p):
     fig, (ax1, ax2) = plt.subplots(1, 2, width_ratios=[1-width_ratios, width_ratios], figsize=fig_p.size)
     fig.subplots_adjust(wspace=0.0)
     color = fig_p.color or ['r']
     linestyle = fig_p.linestyle or ['-']
     linewidth = fig_p.linewidth or [0.8]
 
     ax1.plot(arr, bands.T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
@@ -190,20 +190,20 @@
 
     if num + 1 > len(linewidth):
         linewidth = linewidth + [0.8] * (num + 1 - len(linewidth))
 
     for i in range(num):
         if color[i+1]:
             ax2.plot(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], linewidth=linewidth[i+1], linestyle=linestyle[i+1], color=color[i+1])
-            if fill:
-                plt.fill_between(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], 0, color=color[i+2], alpha=0.2)
+            if fig_p.fill:
+                plt.fill_between(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], 0, color=color[i+2], alpha=fig_p.fill)
         else:
             ax2.plot(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], linewidth=linewidth[i+1], linestyle=linestyle[i+1])
-            if fill:
-                plt.fill_between(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], 0, alpha=0.2)
+            if fig_p.fill:
+                plt.fill_between(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], 0, alpha=fig_p.fill)
 
     ax1.legend(legend, frameon=False, prop={'size':'small'}, loc=fig_p.location)
     ax1.tick_params(axis='y', which='minor', color='gray')
     ax2.minorticks_on()
     ax2.tick_params(axis='both', which='minor', color='gray')
     ax2.set_yticklabels([])
     ax2.legend(p_dos, elements, frameon=False, prop={'size':'small'}, loc=fig_p.location, alignment='left', title="Density of states", title_fontproperties={'size':'small'})
@@ -220,15 +220,15 @@
     ax2.set_xlim(fig_p.horizontal)
     ax2.set_ylim(fig_p.vertical)
     ax1.set_xticks(ticks,labels)
     ax2.tick_params(axis='x', labelsize='x-small', labelcolor='dimgray', labelrotation=-90, pad=1.5)
     ax1.set_ylabel('Energy (eV)')
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
-def IspinWd(arr, bands, ticks, labels, darr, dele, fill, index_f, elements, width_ratios, legend, fig_p):
+def IspinWd(arr, bands, ticks, labels, darr, dele, index_f, elements, width_ratios, legend, fig_p):
     fig, (ax1, ax2) = plt.subplots(1, 2, width_ratios=[1-width_ratios, width_ratios], figsize=fig_p.size)
     fig.subplots_adjust(wspace=0.0)
     color = fig_p.color or ['r', 'k']
     linestyle = fig_p.linestyle or ['-', '-.']
     linewidth = fig_p.linewidth or [0.8, 0.8]
     if len(color) == 1:
         color = [color[0], 'k']
@@ -249,20 +249,20 @@
 
     if num + 2 > len(linewidth):
         linewidth = linewidth + [0.8] * (num + 2 - len(linewidth))
 
     for i in range(num):
         if color[i+2]:
             p_dos = p_dos + ax2.plot(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], linewidth=linewidth[i+2], linestyle=linestyle[i+2], color=color[i+2])
-            if fill:
-                plt.fill_between(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], 0, color=color[i+2], alpha=0.2)
+            if fig_p.fill:
+                plt.fill_between(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], 0, color=color[i+2], alpha=fig_p.fill)
         else:
             p_dos = p_dos + ax2.plot(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], linewidth=linewidth[i+2], linestyle=linestyle[i+2])
-            if fill:
-                plt.fill_between(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], 0, alpha=0.2)
+            if fig_p.fill:
+                plt.fill_between(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], 0, alpha=fig_p.fill)
 
     ax1.tick_params(axis='y', which='minor', color='gray')
     ax2.minorticks_on()
     ax2.tick_params(axis='both', which='minor', color='gray')
     ax2.axvline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.set_yticklabels([])
     ax2.legend(p_dos, elements, frameon=False, prop={'size':'small'}, loc=fig_p.location, alignment='left', title="Density of states", title_fontproperties={'size':'small'})
@@ -278,15 +278,15 @@
     ax2.set_xlim(fig_p.horizontal)
     ax2.set_ylim(fig_p.vertical)
     ax1.set_xticks(ticks,labels)
     ax2.tick_params(axis='x', labelsize='x-small', labelcolor='dimgray', labelrotation=-90, pad=1.5)
     ax1.set_ylabel('Energy (eV)')
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
-def DispinWd(arr, bands, ticks, labels, darr, dele, fill, index_f, elements, width_ratios, legend, fig_p):
+def DispinWd(arr, bands, ticks, labels, darr, dele, index_f, elements, width_ratios, legend, fig_p):
     fig, (ax1, ax2, ax3) = plt.subplots(1, 3, width_ratios=[0.4*(1-width_ratios), 0.4*(1-width_ratios), width_ratios], figsize=fig_p.size)
     fig.subplots_adjust(wspace=0.0)
     color = fig_p.color or ['r', 'k']
     linestyle = fig_p.linestyle or ['-', '-.']
     linewidth = fig_p.linewidth or [0.8, 0.8]
     if len(color) == 1:
         color = [color[0], 'k']
@@ -314,20 +314,20 @@
 
     if num + 2 > len(linewidth):
         linewidth = linewidth + [0.8] * (num + 2 - len(linewidth))
 
     for i in range(num):
         if color[i+2]:
             p_dos = p_dos + ax3.plot(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], linewidth=linewidth[i+2], linestyle=linestyle[i+2], color=color[i+2])
-            if fill:
-                plt.fill_between(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], 0, color=color[i+2], alpha=0.2)
+            if fig_p.fill:
+                plt.fill_between(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], 0, color=color[i+2], alpha=fig_p.fill)
         else:
             p_dos = p_dos + ax3.plot(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], linewidth=linewidth[i+2], linestyle=linestyle[i+2])
-            if fill:
-                plt.fill_between(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], 0, alpha=0.2)
+            if fig_p.fill:
+                plt.fill_between(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], 0, alpha=fig_p.fill)
 
     ax3.axvline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.set_yticklabels([])
     ax3.set_yticklabels([])
     ax3.legend(p_dos, elements, frameon=False, prop={'size':'small'}, loc=fig_p.location, alignment='left', title="Density of states", title_fontproperties={'size':'small'})
 
     ax1.axhline(linewidth=0.4, linestyle='-.', c='gray')
@@ -350,15 +350,15 @@
     else:
         ax1.set_xticks(ticks,labels)
     ax2.set_xticks(ticks,labels)
     ax3.tick_params(axis='x', labelsize='x-small', labelcolor='dimgray', labelrotation=-90, pad=1.5)
     ax1.set_ylabel('Energy (eV)')
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
-def pdosfiles(darr, dele, fill, index_f, elements, legend, exchange, fig_p):
+def pdosfiles(darr, dele, index_f, elements, legend, fig_p):
     plt.figure(figsize=fig_p.size)
     plt.minorticks_on()
     plt.tick_params(axis='both', which='minor', color='gray')
     num = len(index_f)
     p_dos = []
     color = fig_p.color
     linestyle = fig_p.linestyle
@@ -368,54 +368,53 @@
 
     if num > len(linestyle):
         linestyle = linestyle + ['-'] * (num - len(linestyle))
 
     if num > len(linewidth):
         linewidth = linewidth + [0.8] * (num - len(linewidth))
 
-    if exchange:
+    if fig_p.exchange:
         for i in range(num):
             if color[i]:
                 p_dos = p_dos + plt.plot(darr[index_f[i][0]], dele[index_f[i][0]].T[index_f[i][1]], linewidth=linewidth[i], linestyle=linestyle[i], color=color[i])
-                if fill:
-                    plt.fill_between(darr[index_f[i][0]], dele[index_f[i][0]].T[index_f[i][1]], 0, color=color[i], alpha=0.2)
+                if fig_p.fill:
+                    plt.fill_between(darr[index_f[i][0]], dele[index_f[i][0]].T[index_f[i][1]], 0, color=color[i], alpha=fig_p.fill)
             else:
                 p_dos = p_dos + plt.plot(darr[index_f[i][0]], dele[index_f[i][0]].T[index_f[i][1]], linewidth=linewidth[i], linestyle=linestyle[i])
-                if fill:
-                    plt.fill_between(darr[index_f[i][0]], dele[index_f[i][0]].T[index_f[i][1]], 0, alpha=0.2)
+                if fig_p.fill:
+                    plt.fill_between(darr[index_f[i][0]], dele[index_f[i][0]].T[index_f[i][1]], 0, alpha=fig_p.fill)
 
         plt.tick_params(axis='y', labelsize='medium', labelcolor='dimgray')
         plt.xlim(fig_p.vertical)
         plt.ylim(fig_p.horizontal)
         plt.xlabel('Energy (eV)')
         plt.ylabel('Density of states, electrons/eV')
     else:
         for i in range(num):
             if color[i]:
                 p_dos = p_dos + plt.plot(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], linewidth=0.8, linestyle=linestyle[i], color=color[i])
-                if fill:
-                    plt.fill_between(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], 0, color=color[i], alpha=0.2)
+                if fig_p.fill:
+                    plt.fill_between(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], 0, color=color[i], alpha=fig_p.fill)
             else:
                 p_dos = p_dos + plt.plot(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], linewidth=0.8, linestyle=linestyle[i])
-                if fill:
-                    plt.fill_between(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], 0, alpha=0.2)
+                if fig_p.fill:
+                    plt.fill_between(dele[index_f[i][0]].T[index_f[i][1]], darr[index_f[i][0]], 0, alpha=fig_p.fill)
 
         plt.tick_params(axis='x', labelsize='medium', labelcolor='dimgray')
         plt.ylim(fig_p.vertical)
         plt.xlim(fig_p.horizontal)
         plt.ylabel('Energy (eV)')
         plt.xlabel('Density of states, electrons/eV')
 
     plt.axvline(linewidth=0.4, linestyle='-.', c='gray')
     plt.axhline(linewidth=0.4, linestyle='-.', c='gray')
     plt.legend(p_dos, elements, frameon=False, prop={'size':'medium'}, loc=fig_p.location, alignment='left', title=legend[0], title_fontproperties={'size':'medium'})
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
 # pbandplot
-
 def Broken(arr, fre, ticks, labels, broken, height_ratio, legend, fig_p):
     fig, (ax1, ax2) = plt.subplots(2, 1, sharex=True, height_ratios=[height_ratio, 1-height_ratio], figsize=fig_p.size)
     fig.subplots_adjust(hspace=0.0)
     color = fig_p.color or ['r']
     linestyle = fig_p.linestyle or ['-']
     linewidth = fig_p.linewidth or [0.8]
     ax1.plot(arr, fre.T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
@@ -442,14 +441,64 @@
     plt.suptitle('Frequency (THz)', rotation=90, x=0.06, y=0.6, size='medium')
     kwargs = dict(marker=[(-1, -1), (1, 1)], markersize=6,
                   linestyle='', color='k', mec='k', mew=1, clip_on=False)
     ax1.plot([0, 1], [0.02, 0.02], transform=ax1.transAxes, **kwargs)
     ax2.plot([0, 1], [0.98, 0.98], transform=ax2.transAxes, **kwargs)
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
+def Broken2(arr, fre, ticks, labels, broken, height_ratio, legend, fig_p):
+    fig, (ax1, ax2) = plt.subplots(2, 1, sharex=True, height_ratios=[height_ratio, 1-height_ratio], figsize=fig_p.size)
+    fig.subplots_adjust(hspace=0.0)
+    color = fig_p.color or ['r', 'k']
+    linestyle = fig_p.linestyle or ['-', '-.']
+    linewidth = fig_p.linewidth or [0.8, 0.8]
+    if len(color) == 1:
+        color = [color[0], 'k']
+    if len(linestyle) == 1:
+        linestyle = [linestyle[0], '-.']
+    if len(linewidth) == 1:
+        linewidth = [linewidth[0], 0.8]
+    ax1.plot(arr[0], fre[0].T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
+    f = ax2.plot(arr[0], fre[0].T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
+    plt.xlim(arr[0][0], arr[0][-1])
+    vertical = fig_p.vertical or plt.ylim()
+    ax1.set_ylim(broken[1], vertical[1])
+    ax2.set_ylim(vertical[0], broken[0])
+    ax1.spines['bottom'].set_visible(False)
+    ax2.spines['top'].set_visible(False)
+    ax1.xaxis.set_ticks_position(position='none')
+    ax1.tick_params(axis='y', which='minor', color='darkgray')
+    ax1.tick_params(axis='y', labelsize='small', labelcolor='dimgray', labelrotation=-60)
+    ax2.tick_params(axis='y', which='minor', color='gray')
+    ax2.axhline(linewidth=0.4, linestyle='-.', c='gray')
+    if len(ticks) > 2:
+        ticks[0],ticks[-1] = arr[0][0],arr[0][-1]
+        for i in ticks[1:-1]:
+            ax1.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
+            ax2.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
+
+    plt.xticks(ticks,labels)
+    plt.suptitle('Frequency (THz)', rotation=90, x=0.06, y=0.6, size='medium')
+    kwargs = dict(marker=[(-1, -1), (1, 1)], markersize=6,
+                  linestyle='', color='k', mec='k', mew=1, clip_on=False)
+    ax1.plot([0, 1], [0.02, 0.02], transform=ax1.transAxes, **kwargs)
+    ax2.plot([0, 1], [0.98, 0.98], transform=ax2.transAxes, **kwargs)
+    ax1_f = fig.add_subplot(2,1,1)
+    ax1_f.plot(arr[1], fre[1].T, color=color[1], linewidth=linewidth[1], linestyle=linestyle[1])
+    ax1_f.set_xlim(arr[1][0], arr[1][-1])
+    ax1_f.set_ylim(broken[1], vertical[1])
+    ax1_f.axis('off')
+    ax2_f = fig.add_subplot(2,1,2)
+    g = ax2_f.plot(arr[1], fre[1].T, color=color[1], linewidth=linewidth[1], linestyle=linestyle[1])
+    ax2_f.set_xlim(arr[1][0], arr[1][-1])
+    ax2_f.set_ylim(vertical[0], broken[0])
+    ax2_f.axis('off')
+    ax2.legend([f[0], g[0]], [legend[1], legend[2]], frameon=False, prop={'size':'medium'}, loc=fig_p.location, alignment='left', title=legend[0], title_fontproperties={'size':'medium'})
+    plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
+
 def Nobroken(arr, fre, ticks, labels, legend, fig_p):
     plt.figure(figsize=fig_p.size)
     color = fig_p.color or ['r']
     linestyle = fig_p.linestyle or ['-']
     linewidth = fig_p.linewidth or [0.8]
     plt.plot(arr, fre.T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     plt.tick_params(axis='y', which='minor', color='gray')
@@ -462,15 +511,46 @@
     plt.legend(legend, frameon=False, prop={'size':'medium'}, loc=fig_p.location)
     plt.xticks(ticks,labels)
     plt.xlim(arr[0], arr[-1])
     plt.ylim(fig_p.vertical)
     plt.ylabel('Frequency (THz)')
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
-def BrokenWd(arr, fre, ticks, labels, broken, height_ratio, darr, dele, fill, elements, width_ratios, legend, fig_p):
+def Nobroken2(arr, fre, ticks, labels, legend, fig_p):
+    plt.figure(figsize=fig_p.size)
+    color = fig_p.color or ['r', 'k']
+    linestyle = fig_p.linestyle or ['-', '-.']
+    linewidth = fig_p.linewidth or [0.8, 0.8]
+    if len(color) == 1:
+        color = [color[0], 'k']
+    if len(linestyle) == 1:
+        linestyle = [linestyle[0], '-.']
+    if len(linewidth) == 1:
+        linewidth = [linewidth[0], 0.8]
+    f = plt.plot(arr[0], fre[0].T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
+    plt.tick_params(axis='y', which='minor', color='gray')
+    plt.axhline(linewidth=0.4, linestyle='-.', c='gray')
+    if len(ticks) > 2:
+        ticks[0],ticks[-1] = arr[0][0],arr[0][-1]
+        for i in ticks[1:-1]:
+            plt.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
+
+    plt.xticks(ticks,labels)
+    plt.xlim(arr[0][0], arr[0][-1])
+    ylim=plt.ylim(fig_p.vertical)
+    plt.ylabel('Frequency (THz)')
+    ax = plt.axes()
+    g = ax.plot(arr[1], fre[1].T, color=color[1], linewidth=linewidth[1], linestyle=linestyle[1])
+    ax.set_xlim(arr[1][0], arr[1][-1])
+    ax.set_ylim(ylim)
+    ax.axis('off')
+    plt.legend([f[0], g[0]], [legend[1], legend[2]], frameon=False, prop={'size':'medium'}, loc=fig_p.location, alignment='left', title=legend[0], title_fontproperties={'size':'medium'})
+    plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
+
+def BrokenWd(arr, fre, ticks, labels, broken, height_ratio, darr, dele, elements, width_ratios, legend, fig_p):
     fig, ((ax1, ax2), (ax3, ax4)) = plt.subplots(2, 2, height_ratios=[height_ratio, 1-height_ratio], width_ratios=[1-width_ratios, width_ratios], figsize=fig_p.size)
     fig.subplots_adjust(wspace=0.0, hspace=0.0)
     color = fig_p.color or ['r']
     linestyle = fig_p.linestyle or ['-']
     linewidth = fig_p.linewidth or [0.8]
     ax1.plot(arr, fre.T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     ax3.plot(arr, fre.T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
@@ -485,21 +565,21 @@
     if num + 1 > len(linewidth):
         linewidth = linewidth + [0.8] * (num - len(linewidth) + 1)
 
     for i in range(num):
         if color[i+1]:
             ax2.plot(dele[:,i], darr, linewidth=linewidth[i+1], linestyle=linestyle[i+1], color=color[i+1])
             p_dos = p_dos + ax4.plot(dele[:,i], darr, linewidth=linewidth[i+1], linestyle=linestyle[i+1], color=color[i+1])
-            if fill:
-                plt.fill_between(dele[:,i], darr, 0, color=color[i], alpha=0.2)
+            if fig_p.fill:
+                plt.fill_between(dele[:,i], darr, 0, color=color[i], alpha=fig_p.fill)
         else:
             ax2.plot(dele[:,i], darr, linewidth=linewidth[i+1], linestyle=linestyle[i+1])
             p_dos = p_dos + ax4.plot(dele[:,i], darr, linewidth=linewidth[i+1], linestyle=linestyle[i+1])
-            if fill:
-                plt.fill_between(dele[:,i], darr, 0, alpha=0.2)
+            if fig_p.fill:
+                plt.fill_between(dele[:,i], darr, 0, alpha=fig_p.fill)
 
     ax1.set_xlim(arr[0], arr[-1])
     ax3.set_xlim(arr[0], arr[-1])
     vertical = fig_p.vertical or ax1.get_ylim()
 
     ax1.set_ylim(broken[1], vertical[1])
     ax2.set_ylim(broken[1], vertical[1])
@@ -550,15 +630,15 @@
                   linestyle='', color='k', mec='k', mew=1, clip_on=False)
     ax1.plot([0, 1], [0.02, 0.02], transform=ax1.transAxes, **kwargs)
     ax3.plot([0, 1], [0.98, 0.98], transform=ax3.transAxes, **kwargs)
     ax2.plot(1, 0.02, transform=ax2.transAxes, **kwargs)
     ax4.plot(1, 0.98, transform=ax4.transAxes, **kwargs)
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
-def NobrokenWd(arr, fre, ticks, labels, darr, dele, fill, elements, width_ratios, legend, fig_p):
+def NobrokenWd(arr, fre, ticks, labels, darr, dele, elements, width_ratios, legend, fig_p):
     fig, (ax1, ax2) = plt.subplots(1, 2, width_ratios=[1-width_ratios, width_ratios], figsize=fig_p.size)
     fig.subplots_adjust(wspace=0.0)
     color = fig_p.color or ['r']
     linestyle = fig_p.linestyle or ['-']
     linewidth = fig_p.linewidth or [0.8]
     ax1.plot(arr, fre.T, color=color[0], linewidth=linewidth[0], linestyle=linestyle[0])
     num = dele.shape[-1]
@@ -571,20 +651,20 @@
 
     if num + 1 > len(linewidth):
         linewidth = linewidth + [0.8] * (num - len(linewidth) + 1)
 
     for i in range(num):
         if color[i+1]:
             p_dos = p_dos + ax2.plot(dele[:,i], darr, linewidth=linewidth[i+1], linestyle=linestyle[i+1], color=color[i+1])
-            if fill:
-                plt.fill_between(dele[:,i], darr, 0, color=color[i], alpha=0.2)
+            if fig_p.fill:
+                plt.fill_between(dele[:,i], darr, 0, color=color[i], alpha=fig_p.fill)
         else:
             p_dos = p_dos + ax2.plot(dele[:,i], darr, linewidth=linewidth[i+1], linestyle=linestyle[i+1])
-            if fill:
-                plt.fill_between(dele[:,i], darr, 0, alpha=0.2)
+            if fig_p.fill:
+                plt.fill_between(dele[:,i], darr, 0, alpha=fig_p.fill)
 
     ax1.set_xlim(arr[0], arr[-1])
     vertical = fig_p.vertical or ax1.get_ylim()
 
     ax1.set_ylim(vertical)
     ax2.set_ylim(vertical)
     ax2.set_xlim(fig_p.horizontal)
@@ -611,15 +691,15 @@
         for i in ticks[1:-1]:
             ax1.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
 
     ax1.set_xticks(ticks,labels)
     ax1.set_ylabel('Frequency (THz)')
     plt.savefig(fig_p.output, dpi=fig_p.dpi, transparent=True, bbox_inches='tight')
 
-def dosfile(darr, dele, fill, elements, legend, exchange, fig_p):
+def dosfile(darr, dele, elements, legend, fig_p):
     plt.figure(figsize=fig_p.size)
     plt.minorticks_on()
     plt.tick_params(axis='both', which='minor', color='gray')
     num = dele.shape[-1]
     color = fig_p.color
     linestyle = fig_p.linestyle
     linewidth = fig_p.linewidth
@@ -629,40 +709,40 @@
 
     if num > len(linestyle):
         linestyle = linestyle + ['-'] * (num - len(linestyle))
 
     if num > len(linewidth):
         linewidth = linewidth + [0.8] * (num - len(linewidth))
 
-    if exchange:
+    if fig_p.exchange:
         for i in range(num):
             if color[i]:
                 p_dos = p_dos + plt.plot(darr, dele[:,i], linewidth=linewidth[i], linestyle=linestyle[i], color=color[i])
-                if fill:
-                    plt.fill_between(darr, dele[:,i], 0, color=color[i], alpha=0.2)
+                if fig_p.fill:
+                    plt.fill_between(darr, dele[:,i], 0, color=color[i], alpha=fig_p.fill)
             else:
                 p_dos = p_dos + plt.plot(darr, dele[:,i], linewidth=linewidth[i], linestyle=linestyle[i])
-                if fill:
-                    plt.fill_between(darr, dele[:,i], 0, alpha=0.2)
+                if fig_p.fill:
+                    plt.fill_between(darr, dele[:,i], 0, alpha=fig_p.fill)
 
         plt.xlim(fig_p.vertical)
         plt.ylim(fig_p.horizontal)
         plt.xlabel('Frequency (THz)')
         plt.ylabel('Phonon DOS')
         plt.tick_params(axis='y', labelsize='medium', labelcolor='dimgray')
     else:
         for i in range(num):
             if color[i]:
                 p_dos = p_dos + plt.plot(dele[:,i], darr, linewidth=linewidth[i], linestyle=linestyle[i], color=color[i])
-                if fill:
-                    plt.fill_between(dele[:,i], darr, 0, color=color[i], alpha=0.2)
+                if fig_p.fill:
+                    plt.fill_between(dele[:,i], darr, 0, color=color[i], alpha=fig_p.fill)
             else:
                 p_dos = p_dos + plt.plot(dele[:,i], darr, linewidth=linewidth[i], linestyle=linestyle[i])
-                if fill:
-                    plt.fill_between(dele[:,i], darr, 0, alpha=0.2)
+                if fig_p.fill:
+                    plt.fill_between(dele[:,i], darr, 0, alpha=fig_p.fill)
 
         plt.ylim(fig_p.vertical)
         plt.xlim(fig_p.horizontal)
         plt.ylabel('Frequency (THz)')
         plt.xlabel('Phonon DOS')
         plt.tick_params(axis='x', labelsize='medium', labelcolor='dimgray')
```

## bandplot/wrapper.py

```diff
@@ -24,34 +24,37 @@
 ''',
                                      formatter_class=argparse.RawDescriptionHelpFormatter)
     parser.add_argument('-v', "--version",    action="version",     version="bandplot "+__version__+" from "+os.path.dirname(__file__)+' (python'+platform.python_version()+')')
     parser.add_argument('-s', "--size",       type=int,   nargs=2,  help='figure size: width, height')
     parser.add_argument('-b', "--divided",    action='store_true',  help="plot the up and down spin in divided subplot")
     parser.add_argument('-y', "--vertical",   type=float, nargs=2,  help="energy (eV) range, default: [-5.0, 5.0]")
     parser.add_argument('-g', "--legend",     type=str,             nargs='+', help="legend labels", default=[])
-    parser.add_argument('-a', "--location",   type=str.lower,       choices=['best', 'upper right', 'upper left', 'lower left', 'lower right', 'right',
+    parser.add_argument('-L', "--location",   type=str.lower,       choices=['best', 'upper right', 'upper left', 'lower left', 'lower right', 'right',
                                                                              'center left', 'center right', 'lower center', 'upper center', 'center'],
                                                                     help="arrange the legend location, default: best", default='best')
     parser.add_argument('-c', "--color",      type=str,             nargs='+', help="line color: b, blue; g, green; r, red; c, cyan; m, magenta; y, yellow;"+
                                                                                     "k, black; w, white", default=[])
     parser.add_argument('-k', "--linestyle",  type=str,             nargs='+', help="linestyle: solid, dashed, dashdot, dotted or tuple; default: solid",
                                                                                     default=[])
     parser.add_argument('-w', "--linewidth",  type=str,             nargs='+', help="linewidth, default: 0.8", default=[])
+    parser.add_argument('-m', "--mass",       action='store_true',  help='calculate the effective masses')
+    parser.add_argument('-M', "--scale",      type=float,           help='the scale of data for effective masses calculation, default: 0.15', default=0.15)
     parser.add_argument('-i', "--input",      type=str,             nargs='+', help="plot figure from .dat file, default: BAND.dat", default=["BAND.dat"])
     parser.add_argument('-o', "--output",     type=str,             help="plot figure filename, default: BAND.png", default="BAND.png")
     parser.add_argument('-q', "--dpi",        type=int,             help="dpi of the figure, default: 500", default=500)
     parser.add_argument('-j', "--klabels",    type=str,             help="filename of KLABELS, default: KLABELS", default="KLABELS")
     parser.add_argument('-l', "--labels",     type=str.upper,       nargs='+', default=[], help='labels for high-symmetry points, such as X S Y K M')
     parser.add_argument('-d', "--dos",        type=str,             nargs='+', default=[], help="plot DOS from .dat file, or file list")
     parser.add_argument('-x', "--horizontal", type=float, nargs=2,  help="Density of states, electrons/eV range")
     parser.add_argument('-n', "--exchange",   action='store_true',  help="exchange the x and y axes of DOS")
     parser.add_argument('-p', "--partial",    type=str,             nargs='+', default=[], help='the partial DOS to plot, s p d')
     parser.add_argument('-e', "--elements",   type=str,             nargs='+', default=[], help="PDOS labels")
     parser.add_argument('-r', "--wratios",    type=float,           help='width ratio for DOS subplot')
     parser.add_argument('-z', "--fill",       action='store_true',  help='fill a shaded region between PDOS and axis')
+    parser.add_argument('-Z', "--alpha",      type=float,           help='alpha value for filling region, default=0.2', default=0.2)
     parser.add_argument('-f', "--font",       type=str,             help="font to use", default='STIXGeneral')
 
     args = parser.parse_args()
 
     labels = [re.sub("'|‘|’", '′', re.sub('"|“|”', '″', re.sub('^GA[A-Z]+$|^G$', 'Γ', i))) for i in args.labels]
     elements = [re.sub("'|‘|’", '′', re.sub('"|“|”', '″', i)) for i in args.elements]
     dosfiles = [f for i in args.dos for f in glob.glob(i)]
@@ -94,135 +97,169 @@
                 for j in str(factor[i]):
                     formula = formula + '$_'+ j + '$'
             else:
                 formula = formula + symbol[i]
 
     legend = args.legend or [formula] or [pltname]
 
+    ticks   = []
+    klabels = []
+    if os.path.exists(args.klabels):
+        ticks, klabels = readdata.klabels(args.klabels)
+
+    if len(labels) == 0:
+        labels=[re.sub('GAMMA|Gamma|G', 'Γ', re.sub('Undefined|Un|[0-9]', '', i)) for i in klabels]
+
+    if len(ticks) > len(labels):
+        labels = labels + [''] * (len(ticks) - len(labels))
+    elif len(ticks) < len(labels):
+        labels = labels[:len(ticks)]
+
     fig_p = cla_fig(output=args.output, size=args.size, vertical=args.vertical, horizontal=args.horizontal,
-                    color=color, linestyle=linestyle, linewidth=linewidth, location=args.location, dpi=args.dpi)
-    bandfile = [f for i in args.input for f in glob.glob(i)]
-    if len(bandfile) == 1:
+                    color=color, linestyle=linestyle, linewidth=linewidth, location=args.location, dpi=args.dpi,
+                    exchange=args.exchange, fill=args.fill)
+# calculate the effective masses
+    if args.mass:
         if not fig_p.vertical:
             fig_p.vertical = [-5.0, 5.0]
-        arr, bands, ispin = readdata.bands(bandfile[0])
-        ticks   = []
-        klabels = []
-        if os.path.exists(args.klabels):
-            ticks, klabels = readdata.klabels(args.klabels)
-
-        if len(labels) == 0:
-            labels=[re.sub('GAMMA|Gamma|G', 'Γ', re.sub('Undefined|Un|[0-9]', '', i)) for i in klabels]
-
-        if len(ticks) > len(labels):
-            labels = labels + [''] * (len(ticks) - len(labels))
-        elif len(ticks) < len(labels):
-            labels = labels[:len(ticks)]
-
-        if not dosfiles:
-            if ispin == "Noneispin":
-                plots.Noneispin(arr, bands, ticks, labels, legend, fig_p)
-            elif ispin == "Ispin" and not args.divided:
-                plots.Ispin(arr, bands, ticks, labels, legend, fig_p)
-            elif ispin == "Ispin" and args.divided:
-                plots.Dispin(arr, bands, ticks, labels, legend, fig_p)
+        from bandplot import mass
+        if os.path.exists("BAND_GAP"):
+            lumo, homo, homo_c, filename = mass.get_vbm_cbm("BAND_GAP")
+            Extension = [len(lumo), len(homo), len(homo_c), len(filename)]
+            if all(x == 1 for x in Extension):
+                data = mass.bs_dat_read(filename)
+                calM = mass.dat_read(data[0], lumo[0], homo[0], homo_c[0], args.scale)
+                pltlabel = mass.npfit(calM)
+                mass.plot(data[0], calM, pltlabel, ticks, labels, legend, fig_p)
+            elif all(x == 2 for x in Extension):
+                data = mass.bs_dat_read(filename)
+                calM_u = mass.dat_read(data[0], lumo[0], homo[0], homo_c[0], args.scale)
+                calM_d = mass.dat_read(data[1], lumo[1], homo[1], homo_c[1], args.scale)
+                pltlabel_u = mass.npfit(calM_u)
+                pltlabel_d = mass.npfit(calM_d)
+                mass.plot2(data, calM_u, pltlabel_u, calM_d, pltlabel_d, ticks, labels, legend, fig_p)
+            else:
+                print("ERROR: Input file mismatch.")
         else:
-            darr, dele, s_elements = readdata.dos(args.dos)
-            index_f, labels_elements = readdata.select(s_elements, args.partial)
-            if not elements:
-                elements = labels_elements
-            if not args.wratios:
-                if not args.divided:
-                    width_ratios = 0.5
-                else:
-                    width_ratios = 0.3
+            print("ERROR: BAND_GAP file does not exist.")
+# plot Band Structure
+    else:
+        bandfile = [f for i in args.input for f in glob.glob(i)]
+        if len(bandfile) == 1:
+            if not fig_p.vertical:
+                fig_p.vertical = [-5.0, 5.0]
+            arr, bands, ispin = readdata.bands(bandfile[0])
+            if not dosfiles:
+                if ispin == "Noneispin":
+                    plots.Noneispin(arr, bands, ticks, labels, legend, fig_p)
+                elif ispin == "Ispin" and not args.divided:
+                    plots.Ispin(arr, bands, ticks, labels, legend, fig_p)
+                elif ispin == "Ispin" and args.divided:
+                    plots.Dispin(arr, bands, ticks, labels, legend, fig_p)
             else:
-                width_ratios = args.wratios
-
-            if ispin == "Noneispin":
-                plots.NoneispinWd(arr, bands, ticks, labels, darr, dele, args.fill, index_f, elements, width_ratios, legend, fig_p)
-            elif ispin == "Ispin" and not args.divided:
-                plots.IspinWd(arr, bands, ticks, labels, darr, dele, args.fill, index_f, elements, width_ratios, legend, fig_p)
-            elif ispin == "Ispin" and args.divided:
-                plots.DispinWd(arr, bands, ticks, labels, darr, dele, args.fill, index_f, elements, width_ratios, legend, fig_p)
-
-    elif len(bandfile) == 0:
-        if dosfiles:
-            if fig_p.output == "BAND.png":
-                fig_p.output = "DOS.png"
-            darr, dele, s_elements = readdata.dos(dosfiles)
-            index_f, labels_elements = readdata.select(s_elements, args.partial)
-            if not elements:
-                elements = labels_elements
+                darr, dele, s_elements = readdata.dos(args.dos)
+                index_f, labels_elements = readdata.select(s_elements, args.partial)
+                if not elements:
+                    elements = labels_elements
+                if not args.wratios:
+                    if not args.divided:
+                        width_ratios = 0.5
+                    else:
+                        width_ratios = 0.3
+                else:
+                    width_ratios = args.wratios
+                if fig_p.fill:
+                    fig_p.fill = args.alpha
+
+                if ispin == "Noneispin":
+                    plots.NoneispinWd(arr, bands, ticks, labels, darr, dele, index_f, elements, width_ratios, legend, fig_p)
+                elif ispin == "Ispin" and not args.divided:
+                    plots.IspinWd(arr, bands, ticks, labels, darr, dele, index_f, elements, width_ratios, legend, fig_p)
+                elif ispin == "Ispin" and args.divided:
+                    plots.DispinWd(arr, bands, ticks, labels, darr, dele, index_f, elements, width_ratios, legend, fig_p)
+# plot DOS
+        elif len(bandfile) == 0:
+            if dosfiles:
+                if fig_p.output == "BAND.png":
+                    fig_p.output = "DOS.png"
+                darr, dele, s_elements = readdata.dos(dosfiles)
+                index_f, labels_elements = readdata.select(s_elements, args.partial)
+                if not elements:
+                    elements = labels_elements
+                if fig_p.fill:
+                    fig_p.fill = args.alpha
 
-            plots.pdosfiles(darr, dele, args.fill, index_f, elements, legend, args.exchange, fig_p)
+                plots.pdosfiles(darr, dele, index_f, elements, legend, fig_p)
+            else:
+                print("ERROR: No *.dat file.")
+# compare two band structures
+        elif len(bandfile) == 2:
+            if not fig_p.vertical:
+                fig_p.vertical = [-5.0, 5.0]
+            arr = [''] * 2
+            bands = [''] * 2
+            ispin = [''] * 2
+            arr[0], bands[0], ispin[0] = readdata.bands(bandfile[0])
+            arr[1], bands[1], ispin[1] = readdata.bands(bandfile[1])
+            ticks   = []
+            klabels = []
+            if os.path.exists(args.klabels):
+                ticks, klabels = readdata.klabels(args.klabels)
+
+            if len(labels) == 0:
+                labels=[re.sub('GAMMA|Gamma|G', 'Γ', re.sub('Undefined|Un|[0-9]', '', i)) for i in klabels]
+
+            if len(ticks) > len(labels):
+                labels = labels + [''] * (len(ticks) - len(labels))
+            elif len(ticks) < len(labels):
+                labels = labels[:len(ticks)]
+
+            if len(legend) < 3:
+                legend = legend + [''] * (3 - len(legend))
+
+            if all(x == "Noneispin" for x in ispin):
+                plots.Noneispin2(arr, bands, ticks, labels, legend, fig_p)
+            elif all(x == "Ispin" for x in ispin):
+                plots.Dispin2(arr, bands, ticks, labels, legend, fig_p)
         else:
-            print('No .dat file!')
-
-    if len(bandfile) == 2:
-        if not fig_p.vertical:
-            fig_p.vertical = [-5.0, 5.0]
-        arr = [''] * 2
-        bands = [''] * 2
-        ispin = [''] * 2
-        arr[0], bands[0], ispin[0] = readdata.bands(bandfile[0])
-        arr[1], bands[1], ispin[1] = readdata.bands(bandfile[1])
-        ticks   = []
-        klabels = []
-        if os.path.exists(args.klabels):
-            ticks, klabels = readdata.klabels(args.klabels)
-
-        if len(labels) == 0:
-            labels=[re.sub('GAMMA|Gamma|G', 'Γ', re.sub('Undefined|Un|[0-9]', '', i)) for i in klabels]
-
-        if len(ticks) > len(labels):
-            labels = labels + [''] * (len(ticks) - len(labels))
-        elif len(ticks) < len(labels):
-            labels = labels[:len(ticks)]
-
-        if len(legend) < 3:
-            legend = legend + [''] * (3 - len(legend))
-
-        if all(x == "Noneispin" for x in ispin):
-            plots.Noneispin2(arr, bands, ticks, labels, legend, fig_p)
-        elif all(x == "Ispin" for x in ispin):
-            plots.Dispin2(arr, bands, ticks, labels, legend, fig_p)
+            print("Input file mismatch.")
 
 def pmain():
     parser = argparse.ArgumentParser(description='Plot the phonon band structure or DOS from phonopy results.',
                                      epilog='''
 Example:
 pbandplot -i BAND.dat -o BAND.png -l g m k g -d projected_dos.dat -g \$\\pi^2_4\$ -e Si C O
 ''',
                                      formatter_class=argparse.RawDescriptionHelpFormatter)
     parser.add_argument('-v', "--version",    action="version",     version="bandplot "+__version__+" from "+os.path.dirname(__file__)+' (python'+platform.python_version()+')')
     parser.add_argument('-s', "--size",       type=float, nargs=2,  help='figure size: width, height')
     parser.add_argument('-b', "--broken",     type=float, nargs=2,  help='broken axis: start, end')
     parser.add_argument('-r', "--hratios",    type=float,           help='height ratio for broken axis, default: 0.2', default=0.2)
     parser.add_argument('-y', "--vertical",   type=float, nargs=2,  help="frequency (THz) range")
-    parser.add_argument('-g', "--legend",     type=str,   nargs=1,  help="legend labels")
-    parser.add_argument('-a', "--location",   type=str.lower,       choices=['best', 'upper right', 'upper left', 'lower left', 'lower right', 'right',
+    parser.add_argument('-g', "--legend",     type=str,             nargs='+', help="legend labels", default=[])
+    parser.add_argument('-L', "--location",   type=str.lower,       choices=['best', 'upper right', 'upper left', 'lower left', 'lower right', 'right',
                                                                              'center left', 'center right', 'lower center', 'upper center', 'center'],
                                                                     help="arrange the legend location, default: best", default='best')
     parser.add_argument('-c', "--color",      type=str,             nargs='+', help="line color: b, blue; g, green; r, red; c, cyan; m, magenta; y, yellow;"+
                                                                                     "k, black; w, white", default=[])
     parser.add_argument('-k', "--linestyle",  type=str,             nargs='+', help="linestyle: solid, dashed, dashdot, dotted or tuple; default: solid",
                                                                                     default=[])
     parser.add_argument('-w', "--linewidth",  type=str,             nargs='+', help="linewidth, default: 0.8", default=[])
-    parser.add_argument('-i', "--input",      type=str,             help="plot figure from .dat file, default: BAND.dat", default="BAND.dat")
+    parser.add_argument('-i', "--input",      type=str,             nargs='+', help="plot figure from .dat file, default: BAND.dat", default=["BAND.dat"])
     parser.add_argument('-o', "--output",     type=str,             help="plot figure filename, default: BAND.png", default="BAND.png")
     parser.add_argument('-q', "--dpi",        type=int,             help="dpi of the figure, default: 500", default=500)
     parser.add_argument('-j', "--bandconf",   type=str,             help="filename of band setting file, default: band.conf", default="band.conf")
     parser.add_argument('-l', "--labels",     type=str.upper,       nargs='+', default=[], help='labels for high-symmetry points, such as X S Y K M')
     parser.add_argument('-d', "--dos",        type=str,             help="plot Phonon DOS from .dat file")
     parser.add_argument('-x', "--horizontal", type=float, nargs=2,  help="Phonon density of states range")
     parser.add_argument('-n', "--exchange",   action='store_true',  help="exchange the x and y axes of Phonon DOS")
     parser.add_argument('-e', "--elements",   type=str,             nargs='+', default=[], help="PDOS labels")
     parser.add_argument('-p', "--wratios",    type=float,           help='width ratio for DOS subplot, default 0.5', default=0.5)
     parser.add_argument('-z', "--fill",       action='store_true',  help='fill a shaded region between PDOS and axis')
+    parser.add_argument('-Z', "--alpha",      type=float,           help='alpha value for filling region, default=0.2', default=0.2)
     parser.add_argument('-f', "--font",       type=str,             help="font to use", default='STIXGeneral')
 
     args = parser.parse_args()
 
     labels = [re.sub("'|‘|’", '′', re.sub('"|“|”', '″', re.sub('^GA[A-Z]+$|^G$', 'Γ', i))) for i in args.labels]
     elements = [re.sub("'|‘|’", '′', re.sub('"|“|”', '″', i)) for i in args.elements]
     color  = []
@@ -278,17 +315,20 @@
         height_ratio = 0.2
 
     width_ratios = args.wratios
     if width_ratios >= 1 or width_ratios <= 0:
         width_ratios = 0.5
 
     fig_p = cla_fig(output=args.output, size=args.size, vertical=args.vertical, horizontal=args.horizontal,
-                    color=color, linestyle=linestyle, linewidth=linewidth, location=args.location, dpi=args.dpi)
-    if os.path.exists(args.input):
-        arr, fre, ticks = readdata.pbands(args.input)
+                    color=color, linestyle=linestyle, linewidth=linewidth, location=args.location, dpi=args.dpi,
+                    exchange=args.exchange, fill=args.fill)
+# plot Phonon Band Structure
+    bandfile = [f for i in args.input for f in glob.glob(i)]
+    if len(bandfile) == 1:
+        arr, fre, ticks = readdata.pbands(bandfile[0])
         klabels = []
         if os.path.exists(args.bandconf):
             klabels = readdata.bandset(args.bandconf)
         if len(labels) == 0:
             labels=[re.sub('^GA[A-Z]+$|^G$', 'Γ', i) for i in klabels]
         if len(ticks) > len(labels):
             labels = labels + [''] * (len(ticks) - len(labels))
@@ -297,19 +337,46 @@
         if args.dos is None:
             if args.broken is None:
                 plots.Nobroken(arr, fre, ticks, labels, legend, fig_p)
             else:
                 plots.Broken(arr, fre, ticks, labels, broken, height_ratio, legend, fig_p)
         elif os.path.exists(args.dos):
             darr, dele = readdata.pdos(args.dos)
+            if fig_p.fill:
+                fig_p.fill = args.alpha
             if args.broken is None:
-                plots.NobrokenWd(arr, fre, ticks, labels, darr, dele, args.fill, elements, width_ratios, legend, fig_p)
+                plots.NobrokenWd(arr, fre, ticks, labels, darr, dele, elements, width_ratios, legend, fig_p)
             else:
-                plots.BrokenWd(arr, fre, ticks, labels, broken, height_ratio, darr, dele, args.fill, elements, width_ratios, legend, fig_p)
-
-    else:
+                plots.BrokenWd(arr, fre, ticks, labels, broken, height_ratio, darr, dele, elements, width_ratios, legend, fig_p)
+# plot Phonon DOS
+    elif len(bandfile) == 0:
         if args.dos and os.path.exists(args.dos):
             darr, dele = readdata.pdos(args.dos)
-            plots.dosfile(darr, dele, args.fill, elements, legend, args.exchange, fig_p)
+            if fig_p.fill:
+                fig_p.fill = args.alpha
+            plots.dosfile(darr, dele, elements, legend, fig_p)
+        else:
+            print('No *.dat file.')
+# compare two Phonon band structures
+    elif len(bandfile) == 2:
+        arr = [''] * 2
+        fre = [''] * 2
+        ticks = [''] * 2
+        arr[0], fre[0], ticks[0] = readdata.pbands(bandfile[0])
+        arr[1], fre[1], ticks[1] = readdata.pbands(bandfile[1])
+        klabels = []
+        if os.path.exists(args.bandconf):
+            klabels = readdata.bandset(args.bandconf)
+        if len(labels) == 0:
+            labels=[re.sub('^GA[A-Z]+$|^G$', 'Γ', i) for i in klabels]
+        if len(ticks[0]) > len(labels):
+            labels = labels + [''] * (len(ticks[0]) - len(labels))
+        elif len(ticks[0]) < len(labels):
+            labels = labels[:len(ticks[0])]
+        if len(legend) < 3:
+            legend = legend + [''] * (3 - len(legend))
+
+        if args.broken is None:
+            plots.Nobroken2(arr, fre, ticks[0], labels, legend, fig_p)
         else:
-            print('No .dat file!')
+            plots.Broken2(arr, fre, ticks[0], labels, broken, height_ratio, legend, fig_p)
```

## Comparing `bandplot-0.1.4.3.dist-info/METADATA` & `bandplot-0.1.5.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bandplot
-Version: 0.1.4.3
+Version: 0.1.5
 Summary: Band structure, DOS or phonon band structure plot from vaspkit or phonopy result.
 Home-page: https://github.com/lkccrr/bandplot
 Author: kan
 Author-email: luokan@hrbeu.edu.cn
 License: MIT
 Keywords: DFT VASP DOS band plot Phonon
 Platform: Unix
@@ -37,21 +37,21 @@
 The <b style="color:green;"><i>bandplot</b></i> is used for electron band structure, DOS or phonon band structure, DOS plotting from ***vaspkit*** or ***phonopy*** results. The code will provide two scripts, <b style="color:blue;"><i>bandplot</b></i> for band structure or DOS plotting from ***vaspkit*** <b style="color:darkred;"><i>\*.dat</b></i> files, and <b style="color:blue;"><i>pbandplot</b></i> for phonon band structure or DOS plotting from ***phonopy*** <b style="color:darkred;"><i>\*.dat</b></i> files.
 ***
 <b style="color:blue;"><i>bandplot</b></i>
 * To execute <b style="color:blue;"><i>bandplot</b></i> <b style="color:red;"><i>\-h</b></i> for the parameters to use.
 * Example:
 ```bash
 bandplot -h
-bandplot -i BAND.dat -o band.png -l g m k g -d PDOS* -z
+bandplot -i BAND.dat -o BAND.png -l g m k g -d PDOS* -z
 bandplot -i BAND1.dat BAND2.dat -g TiO\$_2\$ PBE HSE
 bandplot -b -l g m k g -y -3 3
 ```
 ***
 <b style="color:blue;"><i>pbandplot</b></i>
 * To execute <b style="color:blue;"><i>pbandplot</b></i> <b style="color:red;"><i>\-h</b></i> for the parameters to use.
 * Example:
 ```bash
 pbandplot -h
-pbandplot -i band.dat -o pband.png -l g m k g -d projected_dos.dat -z
+pbandplot -i BAND.dat -o BAND.png -l g m k g -d projected_dos.dat -z
 pbandplot -b 23 100 -l g m k g -y -2 110
 ```
```

