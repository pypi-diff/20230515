# Comparing `tmp/aligo-5.5.9.tar.gz` & `tmp/aligo-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aligo-5.5.9.tar", last modified: Sat Feb  4 06:04:50 2023, max compression
+gzip compressed data, was "aligo-6.0.0.tar", last modified: Mon May 15 09:02:52 2023, max compression
```

## Comparing `aligo-5.5.9.tar` & `aligo-6.0.0.tar`

### file list

```diff
@@ -1,206 +1,211 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 06:04:50.836366 aligo-5.5.9/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-04 06:04:45.000000 aligo-5.5.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7953 2023-02-04 06:04:50.836366 aligo-5.5.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-02-04 06:04:45.000000 aligo-5.5.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 06:04:50.816366 aligo-5.5.9/aligo/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-02-04 06:04:50.000000 aligo-5.5.9/aligo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 06:04:50.820366 aligo-5.5.9/aligo/apis/
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/apis/Album.py
--rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/apis/Aligo.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/apis/Audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/apis/Compress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/apis/Copy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/apis/Create.py
--rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/apis/CustomShare.py
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/apis/Download.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/apis/Drive.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/apis/Duplicate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8741 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/apis/File.py
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/apis/Move.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/apis/Other.py
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/apis/Recyclebin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/apis/Search.py
--rw-r--r--   0 runner    (1001) docker     (123)    21961 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/apis/Share.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/apis/Star.py
--rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/apis/SyncFolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/apis/Update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/apis/Video.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 06:04:50.820366 aligo-5.5.9/aligo/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/Album.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/Audio.py
--rw-r--r--   0 runner    (1001) docker     (123)    16618 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/Auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    10399 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/BaseAligo.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/Compress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/Config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/Copy.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/Core.py
--rw-r--r--   0 runner    (1001) docker     (123)    12899 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/Create.py
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/Download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/Drive.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/Duplicate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/EMail.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/File.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/LoginServer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/Move.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/Other.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/Recyclebin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/Search.py
--rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/Share.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/Star.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/Template.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/Update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/User.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/Video.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 06:04:50.820366 aligo-5.5.9/aligo/error/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/error/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 06:04:50.828366 aligo-5.5.9/aligo/request/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/AimSearchRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/AlbumListFilesRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/AlbumListRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/ArchiveStatusRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/ArchiveUncompressRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/BatchCancelShareRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/BatchCopyFilesRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/BatchDownloadUrlRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/BatchGetFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/BatchMoveFilesRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/BatchMoveToTrashRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/BatchRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/BatchRestoreRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/BatchShareFileSaveToDriveRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/BatchStarFilesRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/BatchSubRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/CancelShareLinkRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/CompleteFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/CopyFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/CreateFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/CreateFolderRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/CreateShareLinkRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/GetAudioPlayInfoRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/GetDefaultDriveRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/GetDownloadUrlRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/GetDriveRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/GetFileListRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/GetFilePathRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/GetFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/GetRecycleBinListRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/GetShareFileListRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/GetShareFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/GetShareInfoRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/GetShareLinkDownloadUrlRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/GetShareLinkListRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/GetShareTokenRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/GetStarredListRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/GetUploadUrlRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/GetVideoPlayInfoRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/GetVideoPreviewPlayInfoRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/ListToCleanRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/MoveFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/MoveFileToTrashRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/RenameFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/RestoreFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/SearchFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/SearchShareFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/ShareFileSaveToDriveRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/StarredFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/TemplateRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/UpdateFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/UpdateShareLinkRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/request/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 06:04:50.832366 aligo-5.5.9/aligo/response/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/AimSearchResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/AlbumInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/AlbumListResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/ArchiveStatusResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/ArchiveUncompressResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/BatchDownloadUrlResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/BatchShareFileSaveToDriveResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/BatchSubResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/CancelShareLinkResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/CopyFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/CreateFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/CreateShareLinkResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/DuplicateListResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/GetAudioPlayInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/GetDownloadUrlResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/GetFileListResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/GetFilePathResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/GetOfficePreviewUrlResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/GetPersonalInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/GetRecycleBinListResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/GetShareFileListResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/GetShareInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/GetShareLinkDownloadUrlResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/GetShareLinkListResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/GetShareTokenResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/GetStarredListResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/GetUploadUrlResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/GetVideoPlayInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/GetVideoPreviewPlayInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/ListMyDrivesResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/ListResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/ListToCleanResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/MoveFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/MoveFileToTrashResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/RestoreFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/RewardSpaceResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/SearchFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/SearchShareFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/ShareFileSaveToDriveResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/ShareItemInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/ShareLinkExtractCodeResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/TemplateResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/UpdateShareLinkResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/UsersVipInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/response/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 06:04:50.836366 aligo-5.5.9/aligo/types/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/AudioMeta.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/AudioMusicMeta.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/AudioTranscodeTemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/BaseAlbum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/BaseDrive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/BaseFile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/BaseShareFile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/BaseUser.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/CroppingBoundary.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/CroppingSuggestionItem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/DataClass.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/DriveCapacityDetail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/Enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/FaceThumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/FieldsInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/ImageMedia.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/ImageQuality.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/ImageTag.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/ListAlbumItem.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/LoginTimout.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/MediaTransCodeTemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/Null.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/PersonalRightsInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/PersonalSpaceInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/Privilege.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/RateLimit.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/ShareLinkBaseFile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/ShareLinkSchema.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/SystemTag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/Token.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/UploadPartInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/UserConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/VideoMedia.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/VideoMediaAudioStream.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/VideoMediaVideoStream.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/VideoPreview.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/VideoPreviewPlayInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/VideoPreviewSprite.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/VideoTranscodeTemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-02-04 06:04:45.000000 aligo-5.5.9/aligo/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 06:04:50.836366 aligo-5.5.9/aligo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7953 2023-02-04 06:04:50.000000 aligo-5.5.9/aligo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-02-04 06:04:50.000000 aligo-5.5.9/aligo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-04 06:04:50.000000 aligo-5.5.9/aligo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-02-04 06:04:50.000000 aligo-5.5.9/aligo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-04 06:04:50.000000 aligo-5.5.9/aligo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-04 06:04:45.000000 aligo-5.5.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-02-04 06:04:50.836366 aligo-5.5.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:02:52.247851 aligo-6.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-15 09:02:42.000000 aligo-6.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-05-15 09:02:52.247851 aligo-6.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-05-15 09:02:42.000000 aligo-6.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-15 09:02:42.000000 aligo-6.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-15 09:02:42.000000 aligo-6.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 09:02:52.247851 aligo-6.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:02:52.219851 aligo-6.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:02:52.223851 aligo-6.0.0/src/aligo/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-15 09:02:51.000000 aligo-6.0.0/src/aligo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:02:52.223851 aligo-6.0.0/src/aligo/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/apis/Album.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/apis/Aligo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/apis/Audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/apis/Compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/apis/Copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/apis/Create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/apis/CustomShare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/apis/Download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/apis/Drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/apis/Duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/apis/File.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/apis/Move.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/apis/Other.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/apis/Recyclebin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/apis/Search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23039 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/apis/Share.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/apis/Star.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17897 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/apis/SyncFolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/apis/Update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/apis/Video.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:02:52.227851 aligo-6.0.0/src/aligo/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/core/Album.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/core/Audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/core/Auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/core/BaseAligo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/core/Compress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/core/Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/core/Copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/core/Core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12899 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/core/Create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/core/Download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/core/Drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/core/Duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/core/EMail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/core/File.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/core/LoginServer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/core/Move.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/core/Other.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/core/Recyclebin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/core/Search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8958 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/core/Share.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/core/Star.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/core/Template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/core/Update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/core/User.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/core/Video.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:02:52.227851 aligo-6.0.0/src/aligo/error/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/error/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:02:52.235851 aligo-6.0.0/src/aligo/request/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/AimSearchRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/AlbumListFilesRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/AlbumListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/ArchiveStatusRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/ArchiveUncompressRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/BatchCancelShareRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/BatchCopyFilesRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/BatchDownloadUrlRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/BatchGetFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/BatchMoveFilesRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/BatchMoveToTrashRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/BatchRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/BatchRestoreRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/BatchShareFileSaveToDriveRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/BatchStarFilesRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/BatchSubRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/CancelShareLinkRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/CompleteFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/CopyFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/CreateFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/CreateFolderRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/CreateShareLinkRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/GetAudioPlayInfoRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/GetDefaultDriveRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/GetDownloadUrlRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/GetDriveRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/GetFileListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/GetFilePathRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/GetFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/GetRecycleBinListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/GetShareFileListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/GetShareFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/GetShareInfoRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/GetShareLinkDownloadUrlRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/GetShareLinkListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/GetShareTokenRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/GetStarredListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/GetUploadUrlRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/GetVideoPlayInfoRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/GetVideoPreviewPlayInfoRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/ListToCleanRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/MoveFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/MoveFileToTrashRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/RenameFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/RestoreFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/SearchFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/SearchShareFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/ShareFileSaveToDriveRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/StarredFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/TemplateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/UpdateFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/UpdateShareLinkRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/request/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:02:52.243852 aligo-6.0.0/src/aligo/response/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/response/AimSearchResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/response/AlbumInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/response/AlbumListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/response/ArchiveStatusResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/response/ArchiveUncompressResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/response/BatchDownloadUrlResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/response/BatchShareFileSaveToDriveResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/response/BatchSubResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/response/CancelShareLinkResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/response/CopyFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/response/CreateFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/response/CreateShareLinkResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/response/DuplicateListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/response/GetAudioPlayInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/response/GetDownloadUrlResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/response/GetFileListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/response/GetFilePathResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/response/GetOfficePreviewUrlResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/response/GetPersonalInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/response/GetRecycleBinListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/response/GetShareFileListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/response/GetShareInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/response/GetShareLinkDownloadUrlResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/response/GetShareLinkListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/response/GetShareTokenResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/response/GetStarredListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/response/GetUploadUrlResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/response/GetVideoPlayInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/response/GetVideoPreviewPlayInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/response/ListMyDrivesResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/response/ListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/response/ListToCleanResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/response/MoveFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/response/MoveFileToTrashResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/response/RestoreFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/response/RewardSpaceResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/response/SearchFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/response/SearchShareFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/response/ShareFileSaveToDriveResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/response/ShareItemInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/response/ShareLinkExtractCodeResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/response/TemplateResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/response/UpdateShareLinkResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/response/UsersVipInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/response/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:02:52.247851 aligo-6.0.0/src/aligo/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/types/AudioMeta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/types/AudioMusicMeta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/types/AudioTranscodeTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/types/BaseAlbum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/types/BaseDrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/types/BaseFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/types/BaseShareFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/types/BaseUser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/types/CroppingBoundary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/types/CroppingSuggestionItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/types/DataClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/types/DriveCapacityDetail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/types/EMailConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/types/Enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/types/FaceThumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/types/FieldsInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/types/FolderSizeInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/types/ImageMedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/types/ImageQuality.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/types/ImageTag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/types/ListAlbumItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/types/LoginDevice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/types/LoginTimout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/types/MediaTransCodeTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/types/Null.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/types/PersonalRightsInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/types/PersonalSpaceInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/types/Privilege.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/types/RateLimit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/types/ShareLinkBaseFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/types/ShareLinkSchema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/types/SystemTag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/types/Token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/types/UploadPartInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/types/UserConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/types/VideoMedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/types/VideoMediaAudioStream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/types/VideoMediaVideoStream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/types/VideoPreview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/types/VideoPreviewPlayInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/types/VideoPreviewSprite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/types/VideoTranscodeTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-15 09:02:42.000000 aligo-6.0.0/src/aligo/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:02:52.223851 aligo-6.0.0/src/aligo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-05-15 09:02:52.000000 aligo-6.0.0/src/aligo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7074 2023-05-15 09:02:52.000000 aligo-6.0.0/src/aligo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 09:02:52.000000 aligo-6.0.0/src/aligo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-15 09:02:52.000000 aligo-6.0.0/src/aligo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 09:02:52.000000 aligo-6.0.0/src/aligo.egg-info/top_level.txt
```

### Comparing `aligo-5.5.9/LICENSE` & `aligo-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/PKG-INFO` & `aligo-6.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,170 +1,197 @@
 Metadata-Version: 2.1
 Name: aligo
-Version: 5.5.9
-Summary: aliyundrive apis package
-Home-page: https://github.com/foyoux/aligo
-Author: foyou
-Author-email: yimi.0822@qq.com
-License: GPL-3.0
+Version: 6.0.0
+Summary: aliyun drive sdk
+Author: foyoux
 Project-URL: Source, https://github.com/foyoux/aligo
+Project-URL: Homepage, https://github.com/foyoux/aligo
 Project-URL: Bug Tracker, https://github.com/foyoux/aligo/issues
-Description: # aligo
-        
-        🚀🔥 简单、易用、可扩展的阿里云盘 API 接口库 👍👍
-        
-        [wiki 文档](https://github.com/foyoux/aligo/wiki) + [examples](https://github.com/foyoux/aligo/tree/main/examples)
-        
-        > 文档写得很简单，详情请查看 代码提示 + 文档注释
-        > 
-        > 有任何疑问 请 [issue](https://github.com/foyoux/aligo/issues/new?assignees=&labels=&template=bug_report.md&title=)
-        > 或 加入 **aligo交流反馈群** （群二维码在底部）
-        
-        [![python version](https://img.shields.io/pypi/pyversions/aligo)](https://pypi.org/project/aligo/)  [![Downloads](https://static.pepy.tech/personalized-badge/aligo?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/aligo)
-        
-        ```bash
-        pip install --upgrade aligo
-        ```
-        
-        ## 快速入门
-        
-        ```python
-        """快速入门"""
-        from aligo import Aligo
-        
-        if __name__ == '__main__':
-            ali = Aligo()  # 第一次使用，会弹出二维码，供扫描登录
-            
-            user = ali.get_user()  # 获取用户信息
-            print(user.user_name, user.nick_name, user.phone)  # 打印用户信息
-            
-            ll = ali.get_file_list()  # 获取网盘根目录文件列表
-            for file in ll:  # 遍历文件列表
-                print(file.file_id, file.name, file.type)  # 打印文件信息
-        ```
-        
-        https://user-images.githubusercontent.com/35125624/150529002-c2f1b80b-fb11-4e0a-9fd7-6f57f678ccf5.mp4
-        
-        ## 基本功能
-        
-        - [x] 完全的代码提示
-        - [x] 持久化登录、多帐户登录
-        - [x] 福利码兑换
-        - [x] 文件夹同步
-        - [x] 在线解压缩
-        - [x] 支持功能扩展
-        - [x] 搜索文件/标签
-        - [x] 获取重复文件列表
-        - [x] 文件（夹）重命名
-        - [x] 文件（夹）上传下载
-        - [x] 文件（夹）移动复制
-        - [x] 文件（夹）删除恢复
-        - [x] 获取文档在线预览接口
-        - [x] 文件（夹）分享 保存 收藏
-        - [x] 文件（夹）自定义分享（无限制）
-        - [x] 获取帐户、云盘（容量）等基本信息
-        - [x] 相册 创建 删除 修改 添加文件 获取文件
-        - [x] 。。。。。。
-        - [x] ⭐⭐⭐ 欢迎大家发起 [新功能请求](https://github.com/foyoux/aligo/issues/new?assignees=&labels=&template=feature_request.md&title=)
-        
-        > **温馨提示：**
-        >   1. 由于秒传链接的失效，自定分享信息的有效期只有4个小时。
-        >   2. 阿里云盘不同于其他网盘或系统，其定位文件不是基于文件名（路径），而是通过 `file_id`，这才是唯一定位文件的方式，**aligo** 中提供了简便函数 `get_file_by_path`/`get_folder_by_path`，通过网盘路径获取文件对象，通过 其上的 `file_id` 属性即可获取所需文件标识。但不建议频繁使用此方法，因为内部是通过 `get_file_list` 遍历得到的。
-        >   3. 在保存超大分享时（分享中的文件特别多），执行保存全部的方法 - `share_file_save_all_to_drive`，它会立刻执行完毕，但是文件不会立刻被保存到网盘中，阿里云盘服务器会帮你在后台陆续将所有文件存到你的网盘中；所有当你使用 `share_file_save_all_to_drive` 保存超大分享时，却只看到一部分文件时，不用疑惑，这是正常情况。
-        
-        
-        ## 网页扫码登录
-        
-        ```python
-        
-        from aligo import Aligo
-        
-        # 提供 port 参数即可, 之后打开浏览器访问 http://<YOUR_IP>:<port>
-        ali = Aligo(port=8080)
-        ```
-        
-        
-        ## 发送登录二维码到邮箱（推荐）
-        **最佳实践**：建议将邮箱绑定到微信，这样能实时收到提醒，登录过期后也可以第一时间收到登录请求。
-        
-        **安全性问题**：虽然自带公开邮箱（任何人都可以通过此邮箱向你发邮件），但是他人并不能通过这个获取任何人发送的邮件，所以 防伪字符串 策略是安全的。
-        
-        ```python
-        
-        from aligo import Aligo
-        
-        
-        """
-        email: 发送扫码登录邮件 ("接收邮件的邮箱地址", "防伪字符串"). 提供此值时，将不再弹出或打印二维码
-                关于防伪字符串: 为了方便大家使用, aligo 自带公开邮箱, 省去邮箱配置的麻烦.
-                所以收到登录邮件后, 一定要对比确认防伪字符串和你设置一致才可扫码登录, 否则将导致: 包括但不限于云盘文件泄露.
-        """
-        
-        # 提供 email 参数即可
-        ali = Aligo(email=('xxx@qq.com', '防伪字符串，可任意字符串'))
-        ```
-        
-        ## 如何彻底删除文件？
-        > 无需先移动文件到回收站
-        
-        此功能太危险，**aligo** 未直接提供。不过 [这里](https://github.com/foyoux/aligo/wiki/%E8%87%AA%E5%AE%9A%E4%B9%89%E5%8A%9F%E8%83%BD---%E5%BD%BB%E5%BA%95%E5%88%A0%E9%99%A4%E6%96%87%E4%BB%B6) 扩展了该功能，请小心使用！
-        
-        
-        ## 关于扩展功能
-        
-        一般步骤：
-        
-            1. 使用浏览器或其他抓包工具，观察通信过程；
-            2. 获取 url/path + 请求体；
-            3. 继承 `Aligo`, 使用现有的方法 `self._post` 等，进行发送请求；
-            
-        会自动维护 **token**, 你只需关注如何发送请求即可
-        
-        [扩展功能举栗🌰 - 配有视频和代码](https://github.com/foyoux/aligo/issues/24)
-        
-        
-        ## 不慎泄露 refresh_token ?
-        
-        必须马上修改密码！必须马上修改密码！必须马上修改密码！
-        
-        
-        ## 声明
-        
-        此项目仅供学习交流，若有不妥之处，侵联必删。
-        
-        此项目仅供学习交流，若有不妥之处，侵联必删。
-        
-        此项目仅供学习交流，若有不妥之处，侵联必删。
-        
-        ---
-        
-        <table align="center">
-            <thead align="center">
-            <tr>
-                <td><h2>❤️‍🔥欢迎加入🤝🏼</h2></td>
-            </tr>
-            </thead>
-            <tbody align="center">
-            <tr>
-                <td><img src="http://110.42.175.98:5512/down/LKPvT9xK2lFx?fname=/aligo/wechat.jpg" alt="aligo反馈交流群"/></td>
-            </tr>
-            </tbody>
-            <tfoot align="center">
-            <tr>
-                <td>😃 二维码会保持更新 😜</td>
-            </tr>
-            </tfoot>
-        </table>
-Keywords: aligo aliyun drive aliyundrive cloud pcs aliyunpan
-Platform: UNKNOWN
+Keywords: aligo
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Environment :: Console
-Classifier: Natural Language :: Chinese (Simplified)
-Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.7.*
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# aligo
+
+🚀🔥 简单、易用、可扩展的阿里云盘 API 接口库 👍👍
+
+[wiki 文档](https://github.com/foyoux/aligo/wiki) + [examples](https://github.com/foyoux/aligo/tree/main/examples)
+
+> 文档写得很简单，详情请查看 代码提示 + 文档注释
+> 
+> 有任何疑问 请 [issue](https://github.com/foyoux/aligo/issues/new?assignees=&labels=&template=bug_report.md&title=)
+> 或 加入 **aligo交流反馈群** （群二维码在底部）
+
+[![python version](https://img.shields.io/pypi/pyversions/aligo)](https://pypi.org/project/aligo/)  [![Downloads](https://static.pepy.tech/personalized-badge/aligo?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/aligo)
+
+```sh
+pip install -U aligo
+pip install git+https://github.com/foyoux/aligo.git
+```
+
+## 快速入门
+
+```python
+"""快速入门"""
+from aligo import Aligo
+
+if __name__ == '__main__':
+    ali = Aligo()  # 第一次使用，会弹出二维码，供扫描登录
+    
+    user = ali.get_user()  # 获取用户信息
+    print(user.user_name, user.nick_name, user.phone)  # 打印用户信息
+    
+    ll = ali.get_file_list()  # 获取网盘根目录文件列表
+    for file in ll:  # 遍历文件列表
+        print(file.file_id, file.name, file.type)  # 打印文件信息
+```
+
+https://user-images.githubusercontent.com/35125624/150529002-c2f1b80b-fb11-4e0a-9fd7-6f57f678ccf5.mp4
+
+## 基本功能
+
+- [x] 完全的代码提示
+- [x] 持久化登录、多帐户登录
+- [x] 福利码兑换
+- [x] 文件夹同步
+- [x] 在线解压缩
+- [x] 支持功能扩展
+- [x] 搜索文件/标签
+- [x] 获取重复文件列表
+- [x] 文件（夹）重命名
+- [x] 文件（夹）上传下载
+- [x] 文件（夹）移动复制
+- [x] 文件（夹）删除恢复
+- [x] 获取文档在线预览接口
+- [x] 文件（夹）分享 保存 收藏
+- [x] 文件（夹）自定义分享（无限制）
+- [x] 获取帐户、云盘（容量）等基本信息
+- [x] 相册 创建 删除 修改 添加文件 获取文件
+
+更多接口功能，请安装最新版尝试
+
+欢迎大家发起 [新功能请求](https://github.com/foyoux/aligo/issues/new?assignees=&labels=&template=feature_request.md&title=)
+
+> **温馨提示：**
+>   1. 由于秒传链接的失效，自定分享信息的有效期只有4个小时。
+>   2. 阿里云盘不同于其他网盘或系统，其定位文件不是基于文件名（路径），而是通过 `file_id`，这才是唯一定位文件的方式，**aligo** 中提供了简便函数 `get_file_by_path`/`get_folder_by_path`，通过网盘路径获取文件对象，通过 其上的 `file_id` 属性即可获取所需文件标识。但不建议频繁使用此方法，因为内部是通过 `get_file_list` 遍历得到的。
+>   3. 在保存超大分享时（分享中的文件特别多），执行保存全部的方法 - `share_file_save_all_to_drive`，它会立刻执行完毕，但是文件不会立刻被保存到网盘中，阿里云盘服务器会帮你在后台陆续将所有文件存到你的网盘中；所有当你使用 `share_file_save_all_to_drive` 保存超大分享时，却只看到一部分文件时，不用疑惑，这是正常情况。
+
+## 登录
+### 网页扫码登录
+
+```python
+from aligo import Aligo
+
+# 提供 port 参数即可, 之后打开浏览器访问 http://<YOUR_IP>:<port>
+ali = Aligo(port=8080)
+```
+
+
+### 发送登录二维码到邮箱（推荐）
+
+**最佳实践**：建议将邮箱绑定到微信，这样能实时收到提醒，登录过期后也可以第一时间收到登录请求。
+
+```python
+from aligo import Aligo, EMailConfig
+
+if __name__ == '__main__':
+    email_config = EMailConfig(
+        email='<接收登录邮件的邮箱地址>',
+        # 自配邮箱
+        user='',
+        password='',
+        host='',
+        port=0,
+    )
+    ali = Aligo(email=email_config)
+```
+
+## 文件夹同步
+文件夹同步有三种不同的方法，但都可以通过flag参数设置，注意区分。
+```python
+from aligo import Aligo
+
+"""
+flag: 同步标志（类型），默认：None, 另外可选：True, False
+        None：双端同步
+        True：以本地为主
+        False：以云端为主
+"""
+
+ali = Aligo()
+local_folder = 'Path of local'
+remote_id = 'remote id'
+ali.sync_folder(local_folder=local_folder, remote_folder=remote_id,flag=True) 
+```
+
+## 文件上传/下载
+文件的上传与下载有多种不同的实现方法，具体使用请阅读源代码。
+```python
+from aligo import Aligo
+ali = Aligo()
+ali.upload_files(file_paths='file_names' , parent_file_id='reading_id')
+ali.download_file(file_id='<file_id>')
+```
+
+
+## 如何彻底删除文件？
+> 无需先移动文件到回收站
+
+此功能太危险，**aligo** 未直接提供。不过 [这里](https://github.com/foyoux/aligo/wiki/%E8%87%AA%E5%AE%9A%E4%B9%89%E5%8A%9F%E8%83%BD---%E5%BD%BB%E5%BA%95%E5%88%A0%E9%99%A4%E6%96%87%E4%BB%B6) 扩展了该功能，请小心使用！
+
+
+## 关于扩展功能
+
+一般步骤：
+
+    1. 使用浏览器或其他抓包工具，观察通信过程；
+    2. 获取 url/path + 请求体；
+    3. 继承 `Aligo`, 使用现有的方法 `self._post` 等，进行发送请求；
+    
+会自动维护 **token**, 你只需关注如何发送请求即可
+
+[扩展功能举栗🌰 - 配有视频和代码](https://github.com/foyoux/aligo/issues/24)
+
+
+## 不慎泄露 refresh_token ?
+
+虽然官方提供下线功能，但还是要 马上修改密码
+
+今天无意中发现，之前使用 aligo 登录的会在登录设备列表中，但今天发现再使用 aligo 登录，已经不会出现在登录设备列表中，我也不知道为什么
+
+今天把除我手机之外的所有设备下线后，包括 Chrome 和 aligo 登录的，但并没有失效，所有的 token 和 refresh_token 还是可以使用
+
+所以还是得 -> 必须马上修改密码！必须马上修改密码！必须马上修改密码！
+
+
+## 声明
+
+此项目仅供学习交流，若有不妥之处，侵联必删。
+
+---
+
+<table align="center">
+    <thead align="center">
+    <tr>
+        <td><h2>❤️‍🔥欢迎加入🤝🏼</h2></td>
+    </tr>
+    </thead>
+    <tbody align="center">
+    <tr>
+        <td><img src="http://110.42.175.98:5512/down/LKPvT9xK2lFx?fname=/aligo/wechat.jpg" alt="aligo反馈交流群"/></td>
+    </tr>
+    </tbody>
+    <tfoot align="center">
+    <tr>
+        <td>😃 二维码会保持更新 😜</td>
+    </tr>
+    </tfoot>
+</table>
```

### Comparing `aligo-5.5.9/README.md` & `aligo-6.0.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 > 文档写得很简单，详情请查看 代码提示 + 文档注释
 > 
 > 有任何疑问 请 [issue](https://github.com/foyoux/aligo/issues/new?assignees=&labels=&template=bug_report.md&title=)
 > 或 加入 **aligo交流反馈群** （群二维码在底部）
 
 [![python version](https://img.shields.io/pypi/pyversions/aligo)](https://pypi.org/project/aligo/)  [![Downloads](https://static.pepy.tech/personalized-badge/aligo?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/aligo)
 
-```bash
-pip install --upgrade aligo
+```sh
+pip install -U aligo
+pip install git+https://github.com/foyoux/aligo.git
 ```
 
 ## 快速入门
 
 ```python
 """快速入门"""
 from aligo import Aligo
@@ -49,54 +50,82 @@
 - [x] 文件（夹）移动复制
 - [x] 文件（夹）删除恢复
 - [x] 获取文档在线预览接口
 - [x] 文件（夹）分享 保存 收藏
 - [x] 文件（夹）自定义分享（无限制）
 - [x] 获取帐户、云盘（容量）等基本信息
 - [x] 相册 创建 删除 修改 添加文件 获取文件
-- [x] 。。。。。。
-- [x] ⭐⭐⭐ 欢迎大家发起 [新功能请求](https://github.com/foyoux/aligo/issues/new?assignees=&labels=&template=feature_request.md&title=)
+
+更多接口功能，请安装最新版尝试
+
+欢迎大家发起 [新功能请求](https://github.com/foyoux/aligo/issues/new?assignees=&labels=&template=feature_request.md&title=)
 
 > **温馨提示：**
 >   1. 由于秒传链接的失效，自定分享信息的有效期只有4个小时。
 >   2. 阿里云盘不同于其他网盘或系统，其定位文件不是基于文件名（路径），而是通过 `file_id`，这才是唯一定位文件的方式，**aligo** 中提供了简便函数 `get_file_by_path`/`get_folder_by_path`，通过网盘路径获取文件对象，通过 其上的 `file_id` 属性即可获取所需文件标识。但不建议频繁使用此方法，因为内部是通过 `get_file_list` 遍历得到的。
 >   3. 在保存超大分享时（分享中的文件特别多），执行保存全部的方法 - `share_file_save_all_to_drive`，它会立刻执行完毕，但是文件不会立刻被保存到网盘中，阿里云盘服务器会帮你在后台陆续将所有文件存到你的网盘中；所有当你使用 `share_file_save_all_to_drive` 保存超大分享时，却只看到一部分文件时，不用疑惑，这是正常情况。
 
-
-## 网页扫码登录
+## 登录
+### 网页扫码登录
 
 ```python
-
 from aligo import Aligo
 
 # 提供 port 参数即可, 之后打开浏览器访问 http://<YOUR_IP>:<port>
 ali = Aligo(port=8080)
 ```
 
 
-## 发送登录二维码到邮箱（推荐）
-**最佳实践**：建议将邮箱绑定到微信，这样能实时收到提醒，登录过期后也可以第一时间收到登录请求。
+### 发送登录二维码到邮箱（推荐）
 
-**安全性问题**：虽然自带公开邮箱（任何人都可以通过此邮箱向你发邮件），但是他人并不能通过这个获取任何人发送的邮件，所以 防伪字符串 策略是安全的。
+**最佳实践**：建议将邮箱绑定到微信，这样能实时收到提醒，登录过期后也可以第一时间收到登录请求。
 
 ```python
+from aligo import Aligo, EMailConfig
 
-from aligo import Aligo
+if __name__ == '__main__':
+    email_config = EMailConfig(
+        email='<接收登录邮件的邮箱地址>',
+        # 自配邮箱
+        user='',
+        password='',
+        host='',
+        port=0,
+    )
+    ali = Aligo(email=email_config)
+```
 
+## 文件夹同步
+文件夹同步有三种不同的方法，但都可以通过flag参数设置，注意区分。
+```python
+from aligo import Aligo
 
 """
-email: 发送扫码登录邮件 ("接收邮件的邮箱地址", "防伪字符串"). 提供此值时，将不再弹出或打印二维码
-        关于防伪字符串: 为了方便大家使用, aligo 自带公开邮箱, 省去邮箱配置的麻烦.
-        所以收到登录邮件后, 一定要对比确认防伪字符串和你设置一致才可扫码登录, 否则将导致: 包括但不限于云盘文件泄露.
+flag: 同步标志（类型），默认：None, 另外可选：True, False
+        None：双端同步
+        True：以本地为主
+        False：以云端为主
 """
 
-# 提供 email 参数即可
-ali = Aligo(email=('xxx@qq.com', '防伪字符串，可任意字符串'))
+ali = Aligo()
+local_folder = 'Path of local'
+remote_id = 'remote id'
+ali.sync_folder(local_folder=local_folder, remote_folder=remote_id,flag=True) 
 ```
 
+## 文件上传/下载
+文件的上传与下载有多种不同的实现方法，具体使用请阅读源代码。
+```python
+from aligo import Aligo
+ali = Aligo()
+ali.upload_files(file_paths='file_names' , parent_file_id='reading_id')
+ali.download_file(file_id='<file_id>')
+```
+
+
 ## 如何彻底删除文件？
 > 无需先移动文件到回收站
 
 此功能太危险，**aligo** 未直接提供。不过 [这里](https://github.com/foyoux/aligo/wiki/%E8%87%AA%E5%AE%9A%E4%B9%89%E5%8A%9F%E8%83%BD---%E5%BD%BB%E5%BA%95%E5%88%A0%E9%99%A4%E6%96%87%E4%BB%B6) 扩展了该功能，请小心使用！
 
 
 ## 关于扩展功能
@@ -110,22 +139,24 @@
 会自动维护 **token**, 你只需关注如何发送请求即可
 
 [扩展功能举栗🌰 - 配有视频和代码](https://github.com/foyoux/aligo/issues/24)
 
 
 ## 不慎泄露 refresh_token ?
 
-必须马上修改密码！必须马上修改密码！必须马上修改密码！
+虽然官方提供下线功能，但还是要 马上修改密码
 
+今天无意中发现，之前使用 aligo 登录的会在登录设备列表中，但今天发现再使用 aligo 登录，已经不会出现在登录设备列表中，我也不知道为什么
 
-## 声明
+今天把除我手机之外的所有设备下线后，包括 Chrome 和 aligo 登录的，但并没有失效，所有的 token 和 refresh_token 还是可以使用
 
-此项目仅供学习交流，若有不妥之处，侵联必删。
+所以还是得 -> 必须马上修改密码！必须马上修改密码！必须马上修改密码！
 
-此项目仅供学习交流，若有不妥之处，侵联必删。
+
+## 声明
 
 此项目仅供学习交流，若有不妥之处，侵联必删。
 
 ---
 
 <table align="center">
     <thead align="center">
@@ -139,8 +170,8 @@
     </tr>
     </tbody>
     <tfoot align="center">
     <tr>
         <td>😃 二维码会保持更新 😜</td>
     </tr>
     </tfoot>
-</table>
+</table>
```

### Comparing `aligo-5.5.9/aligo/apis/Album.py` & `aligo-6.0.0/src/aligo/apis/Album.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """..."""
-from typing import List
+from typing import List, Union
 
 from aligo.core import *
 from aligo.core.Config import *
 from aligo.request import AlbumListRequest, AlbumListFilesRequest
 from aligo.types import ListAlbumItem, BaseAlbum, BaseFile
 from aligo.types.Enum import *
 
@@ -39,23 +39,20 @@
         return self._result(response, BaseAlbum)
 
     def get_album(self, album_id: str) -> BaseAlbum:
         """获取相册，通过 album_id"""
         response = self._post(ADRIVE_V1_ALBUM_GET, body={'album_id': album_id})
         return self._result(response, BaseAlbum)
 
-    def add_files_to_album(self, album_id: str, files: List[BaseFile]) -> List[BaseFile]:
-        response = self._post('/adrive/v1/album/add_files', body={
+    def add_files_to_album(self, album_id: str, files: List[Union[BaseFile, str]]) -> List[BaseFile]:
+        response = self._post(ADRIVE_V1_ALBUM_ADD_FILES, body={
             'album_id': album_id,
             'drive_file_list': [{'drive_id': f.drive_id, 'file_id': f.file_id} for f in files]
         })
-        return response.json()['file_list']
-
-    def add_file_to_album(self, album_id: str, file: BaseFile) -> BaseFile:
-        return self.add_files_to_album(album_id, [file])[0]
+        return self._result(response, BaseFile, field='file_list')
 
     def list_album_files(self, album_id: str, order_direction: OrderDirection = 'DESC') -> List[BaseFile]:
         """获取指定相册文件"""
         body = AlbumListFilesRequest(album_id=album_id, order_direction=order_direction)
         result = self._core_list_album_files(body)
         return list(result)
```

### Comparing `aligo-5.5.9/aligo/apis/Audio.py` & `aligo-6.0.0/src/aligo/apis/Audio.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/apis/Compress.py` & `aligo-6.0.0/src/aligo/apis/Compress.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/apis/Copy.py` & `aligo-6.0.0/src/aligo/apis/Copy.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/apis/Create.py` & `aligo-6.0.0/src/aligo/apis/Create.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Create class"""
 import os
-from typing import List
+from typing import List, Callable
 
 from aligo.core import *
 from aligo.request import *
 from aligo.response import *
 from aligo.types import *
 from aligo.types.Enum import *
 
@@ -59,30 +59,31 @@
         for file_path in file_paths:
             file = self.upload_file(file_path=file_path, parent_file_id=parent_file_id, drive_id=drive_id,
                                     check_name_mode=check_name_mode)
             file_list.append(file)
         return file_list
 
     def upload_folder(self, folder_path: str, parent_file_id: str = 'root', drive_id: str = None,
-                      check_name_mode: CheckNameMode = "auto_rename",
-                      folder_check_name_mode: CheckNameMode = 'refuse') -> List:
+                      check_name_mode: CheckNameMode = "auto_rename", folder_check_name_mode: CheckNameMode = 'refuse',
+                      file_filter: Callable[[os.DirEntry], bool] = lambda x: False) -> List:
         """
         上传文件夹
         :param folder_path: [str] 文件夹路径
         :param parent_file_id: Optional[str] 父文件夹id, 默认为 'root'
         :param drive_id: [str] 指定网盘id, 默认为 None, 如果为 None, 则使用默认网盘
         :param check_name_mode: [CheckNameMode] 检查文件名模式, 默认为 'auto_rename'
         :param folder_check_name_mode: [CheckNameMode] 检查文件夹名模式, 默认为 'refuse'
+        :param file_filter: 文件过滤函数
         :return: [List]
 
         用法示例:
         >>> from aligo import Aligo
         >>> ali = Aligo()
         >>> # noinspection PyShadowingNames
-        >>> resut = ali.upload_folder('/Users/aligo/Desktop/test')
+        >>> result = ali.upload_folder('/Users/aligo/Desktop/test')
         >>> print(result)
         """
         result = []
         folder_path = os.path.abspath(folder_path)
 
         # 0. 判断是否为文件夹
         if not os.path.isdir(folder_path):
@@ -93,14 +94,16 @@
         folder_name = os.path.basename(folder_path)
         # 2. 在指定 parent_file_id 下创建 folder_name 文件夹, 并获取 folder BaseFile 对象
         folder = self.create_folder(folder_name, parent_file_id=parent_file_id, drive_id=drive_id,
                                     check_name_mode=folder_check_name_mode)
         # 3. 开始扫描目标文件夹
         file: os.DirEntry
         for file in os.scandir(folder_path):
+            if file_filter(file):
+                continue
             if file.is_file():
                 # 4. 如果是文件, 就上传, 并继续
                 x = self.upload_file(file.path, parent_file_id=folder.file_id, name=file.name, drive_id=drive_id,
                                      check_name_mode=check_name_mode)
                 result.append(x)
                 continue
             # 5. 否则为文件夹, 递归
```

### Comparing `aligo-5.5.9/aligo/apis/CustomShare.py` & `aligo-6.0.0/src/aligo/apis/CustomShare.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         """..."""
         result = []
         for file in files:
             result.append({
                 'name': file.name,
                 'content_hash': file.content_hash,
                 'size': file.size,
-                'url': file.download_url
+                'url': file.download_url or file.url
             })
         return result
 
     @staticmethod
     def share_file_by_aligo(file: BaseFile) -> str:
         """
         自定义分享文件
```

### Comparing `aligo-5.5.9/aligo/apis/Download.py` & `aligo-6.0.0/src/aligo/apis/Download.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """..."""
 import os
-from typing import List, overload
+from typing import List, overload, Callable
 
 from aligo.core import *
+from aligo.error import AligoException
 from aligo.request import *
 from aligo.response import *
 from aligo.types import *
 
 
 class Download(Core):
     """..."""
@@ -60,39 +61,44 @@
             drive_id=drive_id,
             file_id_list=file_id_list,
             expire_sec=expire_sec
         )
         result = self._core_batch_download_url(body)
         return list(result)
 
-    def download_folder(self, folder_file_id: str, local_folder: str = '.', drive_id: str = None) -> str:
+    def download_folder(self, folder_file_id: str, local_folder: str = '.', drive_id: str = None,
+                        file_filter: Callable[[BaseFile], bool] = lambda x: False) -> str:
         """
         下载文件夹
         :param folder_file_id: [str] 文件夹 id
         :param local_folder: [str] 本地文件夹路径, 默认为当前目录, 即下载到哪里
         :param drive_id: [str] 文件夹所在的网盘 id
+        :param file_filter: 文件过滤函数
         :return: [str] 本地文件夹路径
 
         用法示例:
         >>> from aligo import Aligo
         >>> ali = Aligo()
         >>> result = ali.download_folder(folder_file_id='<folder_file_id>')
         >>> print(result)
         """
         if folder_file_id != 'root':
             folder = self._core_get_file(GetFileRequest(file_id=folder_file_id, drive_id=drive_id))
             local_folder = os.path.join(local_folder, self._del_special_symbol(folder.name))
-        return self.__download_folder(folder_file_id, local_folder, drive_id)
+        return self.__download_folder(folder_file_id, local_folder, drive_id, file_filter=file_filter)
 
-    def __download_folder(self, folder_file_id: str, local_folder: str = '.', drive_id: str = None) -> str:
+    def __download_folder(self, folder_file_id: str, local_folder: str = '.', drive_id: str = None,
+                          file_filter: Callable[[BaseFile], bool] = lambda x: False) -> str:
         """下载文件夹"""
         # 创建文件夹, 即使文件夹为空
         os.makedirs(local_folder, exist_ok=True)
         files = []
         for file in self._core_get_file_list(GetFileListRequest(parent_file_id=folder_file_id, drive_id=drive_id)):
+            if file_filter(file):
+                continue
             if file.type == 'folder':
                 self.__download_folder(folder_file_id=file.file_id,
                                        local_folder=os.path.join(local_folder, self._del_special_symbol(file.name)))
                 continue
             files.append(file)
         self.download_files(files, local_folder=local_folder)
         return os.path.abspath(local_folder)
@@ -150,11 +156,13 @@
             file: BaseFile = None, drive_id=None
     ) -> str:
         """download_file"""
         if file_id:
             file = self._core_get_file(GetFileRequest(file_id=file_id, drive_id=drive_id))
 
         if file:
+            if file.type == 'folder':
+                raise AligoException('文件类型不对：期待文件，得到的是文件夹')
             file_path = os.path.join(local_folder, file.name)
-            url = file.download_url
+            url = file.download_url or file.url
 
         return self._core_download_file(file_path, url)
```

### Comparing `aligo-5.5.9/aligo/apis/Drive.py` & `aligo-6.0.0/src/aligo/apis/Drive.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/apis/Duplicate.py` & `aligo-6.0.0/src/aligo/apis/Duplicate.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/apis/File.py` & `aligo-6.0.0/src/aligo/apis/File.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """文件相关"""
 import os
 from typing import List, overload, Union, Callable
 
 from aligo.core import *
+from aligo.core.Config import *
 from aligo.request import *
 from aligo.response import *
 from aligo.types import *
 from aligo.types.Enum import *
 
 
 class File(Core):
@@ -217,7 +218,12 @@
         :return:
         """
         for f in self._core_get_file_list(GetFileListRequest(parent_file_id=parent_file_id, drive_id=drive_id)):
             if f.type == 'file':
                 callback(_path, f)
                 continue
             self.walk_files(callback, parent_file_id=f.file_id, drive_id=drive_id, _path=os.path.join(_path, f.name))
+
+    def get_folder_size_info(self, file_id: str, drive_id: str = None) -> FolderSizeInfo:
+        """获取文件夹信息，文件夹个数，以及文件个数及其大小，不递归"""
+        response = self._post(ADRIVE_V1_FILE_GET_FOLDER_SIZE_INFO, body={'file_id': file_id, 'drive_id': drive_id})
+        return self._result(response, FolderSizeInfo)
```

### Comparing `aligo-5.5.9/aligo/apis/Move.py` & `aligo-6.0.0/src/aligo/apis/Move.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/apis/Other.py` & `aligo-6.0.0/src/aligo/apis/Other.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/apis/Recyclebin.py` & `aligo-6.0.0/src/aligo/apis/Recyclebin.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/apis/Search.py` & `aligo-6.0.0/src/aligo/apis/Search.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,21 +44,25 @@
         用法示例：
         >>> from aligo import Aligo, SearchFileRequest
         >>> ali = Aligo()
         >>> files = ali.search_files(body=SearchFileRequest(query='name match "test"'))
         >>> print(files)
         """
 
-    def search_files(self, name: str = None, category: SearchCategory = None, drive_id: str = None,
-                     body: SearchFileRequest = None, **kwargs) -> List[BaseFile]:
+    def search_files(self, name: str = None, category: SearchCategory = None, parent_file_id: str = 'root',
+                     drive_id: str = None, body: SearchFileRequest = None, **kwargs) -> List[BaseFile]:
         """search files"""
         if body is None:
             query = None
+            if parent_file_id != 'root':
+                query = f'parent_file_id = "{parent_file_id}"'
             if name:
-                query = f'name match "{name}"'
+                if query:
+                    query += ' and '
+                query += f'name match "{name}"'
             if category is not None:
                 if query:
                     query += ' and '
                 query += f'category = "{category}"'
             body = SearchFileRequest(query=query, drive_id=drive_id, **kwargs)
         result = self._core_search_files(body)
         return list(result)
```

### Comparing `aligo-5.5.9/aligo/apis/Share.py` & `aligo-6.0.0/src/aligo/apis/Share.py`

 * *Files 8% similar despite different names*

```diff
@@ -263,14 +263,28 @@
         """get_share_file_list"""
         _deprecation_warning(kwargs)
         if body is None:
             body = GetShareFileListRequest(share_id=share_token.share_id, parent_file_id=parent_file_id, **kwargs)
         result = self._core_get_share_file_list(body, share_token)
         return list(result)
 
+    def list_by_share(
+            self,
+            share_token: GetShareTokenResponse = None,
+            parent_file_id: str = 'root',
+            body: GetShareFileListRequest = None,
+            **kwargs
+    ) -> List[BaseShareFile]:
+        """get_share_file_list"""
+        _deprecation_warning(kwargs)
+        if body is None:
+            body = GetShareFileListRequest(share_id=share_token.share_id, parent_file_id=parent_file_id, **kwargs)
+        result = self._core_list_by_share(body, share_token)
+        return list(result)
+
     @overload
     def get_share_file(
             self,
             file_id: str,
             share_token: GetShareTokenResponse,
             **kwargs
     ) -> BaseShareFile:
@@ -320,14 +334,27 @@
     ) -> BaseShareFile:
         """get_share_file"""
         _deprecation_warning(kwargs)
         if body is None:
             body = GetShareFileRequest(share_id=share_token.share_id, file_id=file_id, **kwargs)
         return self._core_get_share_file(body, share_token)
 
+    def get_by_file(
+            self,
+            file_id: str = None,
+            share_token: GetShareTokenResponse = None,
+            body: GetShareFileRequest = None,
+            **kwargs
+    ) -> BaseShareFile:
+        """get_share_file"""
+        _deprecation_warning(kwargs)
+        if body is None:
+            body = GetShareFileRequest(share_id=share_token.share_id, file_id=file_id, **kwargs)
+        return self._core_get_by_share(body, share_token)
+
     @overload
     def get_share_link_download_url(
             self,
             file_id: str,
             share_token: GetShareTokenResponse,
             **kwargs
     ) -> GetShareLinkDownloadUrlResponse:
@@ -536,21 +563,22 @@
         result = self._core_batch_share_file_saveto_drive(body, share_token)
         return list(result)
 
     def share_file_save_all_to_drive(
             self,
             share_token: GetShareTokenResponse,
             to_parent_file_id: str = 'root',
+            parent_file_id: str = 'root',
             auto_rename: bool = True,
             to_drive_id: str = None,
             **kwargs,
     ) -> List[BatchShareFileSaveToDriveResponse]:
         """保存所有分享文件到云盘"""
         _deprecation_warning(kwargs)
-        file_list = self.get_share_file_list(share_token)
+        file_list = self.get_share_file_list(share_token, parent_file_id=parent_file_id)
         result = self.batch_share_file_saveto_drive(
             [file.file_id for file in file_list],
             share_token,
             to_parent_file_id=to_parent_file_id,
             to_drive_id=to_drive_id,
             auto_rename=auto_rename,
         )
```

### Comparing `aligo-5.5.9/aligo/apis/Star.py` & `aligo-6.0.0/src/aligo/apis/Star.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/apis/SyncFolder.py` & `aligo-6.0.0/src/aligo/apis/SyncFolder.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,16 +66,16 @@
             self._auth.log.info('sync_folder: 双端同步')
         elif flag:
             self._auth.log.info('sync_folder: 本地为主')
         else:
             self._auth.log.info('sync_folder: 云端为主')
 
         if not os.path.exists(local_folder):
-            self._auth.log.warning('本地文件夹不存在: %s', local_folder)
-            return
+            self._auth.log.warning('本地文件夹不存在，创建: %s', local_folder)
+            os.makedirs(local_folder)
         self.__sync_folder(local_folder, remote_folder, flag, file_filter, ignore_content, follow_delete, drive_id)
 
     def __sync_folder(
             self,
             local_folder: str,
             remote_folder: str,
             flag: Optional[bool],
```

### Comparing `aligo-5.5.9/aligo/apis/Update.py` & `aligo-6.0.0/src/aligo/apis/Update.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/apis/Video.py` & `aligo-6.0.0/src/aligo/apis/Video.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/core/Album.py` & `aligo-6.0.0/src/aligo/core/Album.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/core/Auth.py` & `aligo-6.0.0/src/aligo/core/Auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 import base64
 import json
 import logging
 import os
 import sys
 import tempfile
 import time
+import uuid
 from dataclasses import asdict
 from http.server import HTTPServer
 from pathlib import Path
-from typing import Callable, overload, List, Dict, Tuple
+from typing import Callable, overload, List, Dict
 
 import coloredlogs
 import qrcode
 import qrcode_terminal
 import requests
 
+import aligo
 from aligo.core.Config import *
 from aligo.error import AligoStatus500, AligoRefreshFailed, AligoFatalError
 from aligo.types import *
 from aligo.types.Enum import *
 from .EMail import send_email
 from .LoginServer import LoginServer
 
@@ -41,22 +43,22 @@
     """退出登录"""
     (aligo_config_folder / f'{name}.json').unlink()
 
 
 class Auth:
     """..."""
 
+    _VERIFY_SSL = True
     _SLEEP_TIME_SEC = None
 
-    # 发送邮件配置
-    _EMAIL_USER = 'aligo_notify@163.com'
-    # noinspection SpellCheckingInspection
-    _EMAIL_PASSWORD = 'IYMQTISDOZYUMUFX'
-    _EMAIL_HOST = 'smtp.163.com'
-    _EMAIL_PORT = 465
+    # x-headers
+    _X_PUBLIC_KEY = ('04d9d2319e0480c840efeeb75751b86d0db0c5b9e72c6260a1d846958adceaf9d'
+                     'ee789cab7472741d23aafc1a9c591f72e7ee77578656e6c8588098dea1488ac2a')
+    _X_SIGNATURE = ('f4b7bed5d8524a04051bd2da876dd79afe922b8205226d65855d02b267422adb1'
+                    'e0d8a816b021eaf5c36d101892180f79df655c5712b348c2a540ca136e6b22001')
 
     def debug_log(self, response: requests.Response):
         """打印错误日志, 便于分析调试"""
         r = response.request
         self.log.warning(f'[method status_code] {r.method} {response.status_code}')
         self.log.warning(f'[url] {response.url}')
         self.log.warning(f'[response body] {response.text[:200]}')
@@ -71,59 +73,57 @@
     def __init__(
             self,
             name: str = 'aligo',
             show: Callable[[str], None] = None,
             level=logging.DEBUG,
             proxies: Dict = None,
             port: int = None,
-            email: Tuple[str, str] = None,
+            email: EMailConfig = None,
             request_failed_delay: float = 3,
             requests_timeout: float = None,
     ):
         """扫描二维码登录"""
 
     @overload
     def __init__(
             self,
             name: str = 'aligo',
             refresh_token: str = None,
             level=logging.DEBUG,
             proxies: Dict = None,
             port: int = None,
-            email: Tuple[str, str] = None,
+            email: EMailConfig = None,
             request_failed_delay: float = 3,
             requests_timeout: float = None,
     ):
         """refresh_token 登录"""
 
     # noinspection PyPep8Naming,SpellCheckingInspection
     def __init__(
             self, name: str = 'aligo',
             refresh_token: str = None,
             show: Callable[[str], None] = None,
             level: int = logging.DEBUG,
             proxies: Dict = None,
             port: int = None,
-            email: Tuple[str, str] = None,
+            email: EMailConfig = None,
             request_failed_delay: float = 3,
             requests_timeout: float = None,
             login_timeout: float = None,
             re_login: bool = True,
     ):
         """登录验证
 
         :param name: (可选, 默认: aligo) 配置文件名称, 便于使用不同配置文件进行身份验证
         :param refresh_token:
         :param show: (可选) 显示二维码的函数
         :param level: (可选) 控制控制台输出
         :param proxies: (可选) 自定义代理 [proxies={"https":"localhost:10809"}],支持 http 和 socks5（具体参考requests库的用法）
         :param port: (可选) 开启 http server 端口，用于网页端扫码登录. 提供此值时，将不再弹出或打印二维码
-        :param email: (可选) 发送扫码登录邮件 ("接收邮件的邮箱地址", "防伪字符串"). 提供此值时，将不再弹出或打印二维码
-            关于防伪字符串: 为了方便大家使用, aligo 自带公开邮箱, 省去邮箱配置的麻烦.
-                        所以收到登录邮件后, 一定要对比确认防伪字符串和你设置一致才可扫码登录, 否则将导致: 包括但不限于云盘文件泄露.
+        :param email: (可选) 邮箱配置，参考 EMailConfig
         :param request_failed_delay: 请求失败后，延迟时间，单位：秒
         :param requests_timeout: same as requests timeout
         :param login_timeout: 登录超时时间，单位：秒
         :param re_login: refresh_token 失效后是否继续登录（弹出二维码或邮件，需等待） fix #73
         """
         self._name_name = name
         self._name = aligo_config_folder.joinpath(f'{name}.json')
@@ -144,64 +144,79 @@
             milliseconds=True,
             datefmt='%X',
             fmt=fmt
         )
 
         self.log.info(f'Config {self._name}')
         self.log.info(f'日志等级 {logging.getLevelName(level)}')
+        self.log.info(f'aligo 版本 {aligo.__version__}')
 
         #
         self.session = requests.session()
         self.session.trust_env = False
         self.session.proxies = proxies
         self.session.headers.update(UNI_HEADERS)
 
-        self.session.get(AUTH_HOST + V2_OAUTH_AUTHORIZE, params={
-            'login_type': 'custom',
-            'response_type': 'code',
-            'redirect_uri': 'https://www.aliyundrive.com/sign/callback',
-            'client_id': CLIENT_ID,
-            'state': r'{"origin":"file://"}',
-            # 'state': '{"origin":"https://www.aliyundrive.com"}',
-        }, stream=True).close()
-
-        #
-        SESSIONID = self.session.cookies.get('SESSIONID')
-        # self.log.debug(f'SESSIONID {SESSIONID}')
-
-        #
         self.token: Optional[Token] = None
-        if show is None:
-            if os.name == 'nt':
-                self.log.info('Windows 操作系统')
-                show = self._show_qrcode_in_window
-            elif sys.platform.startswith('darwin'):
-                self.log.info('MacOS 操作系统')
-                show = self._show_qrcode_in_window
-            else:
-                self.log.info('类 Unix 操作系统')
-                show = self._show_console
+        if os.name == 'nt':
+            self._os_name = 'Windows 操作系统'
+            show = show or self._show_qrcode_in_window
+        elif sys.platform.startswith('darwin'):
+            self._os_name = 'MacOS 操作系统'
+            show = show or self._show_qrcode_in_window
+        else:
+            self._os_name = '类 Unix 操作系统'
+            show = show or self._show_console
+        self.log.info(self._os_name)
         self._show = show
 
-        if refresh_token:
-            self.log.debug('登录方式 refresh_token')
-            self._refresh_token(refresh_token)
-            return
+        self._x_device_id = None
 
         if self._name.exists():
             self.log.info(f'加载配置文件 {self._name}')
             self.token = DataClass.fill_attrs(Token, json.load(self._name.open(encoding='utf8')))
-        else:
+            self.session.headers.update({
+                'Authorization': self.token.access_token,
+            })
+            self._init_x_headers()
+        elif refresh_token is None:
             self.log.info('登录方式 扫描二维码')
             self._login()
 
-        #
+        if refresh_token:
+            self.log.debug('登录方式 refresh_token')
+            self._refresh_token(refresh_token)
+
+    def _create_session(self):
+        self.post(USERS_V1_USERS_DEVICE_CREATE_SESSION, body={
+            'deviceName': f'aligo - {self._name_name}',
+            'modelName': self._os_name,
+            'pubKey': self._X_PUBLIC_KEY,
+        })
+
+    def _renew_session(self):
+        self.post(USERS_V1_USERS_DEVICE_RENEW_SESSION, body={})
+
+    def _init_x_headers(self):
+        if self._x_device_id is None:
+            # 如果 self._x_device_id 为 None，尝试从 token 中获取（来自文件）
+            self._x_device_id = self.token.x_device_id
+        if self._x_device_id is None:
+            # 如果文件中未存储，则说明还没有，则生成
+            self._x_device_id = uuid.uuid4().hex
+        # 设置 x-headers
         self.session.headers.update({
-            'Authorization': self.token.access_token
+            'x-device-id': self._x_device_id,
+            'x-signature': self._X_SIGNATURE
         })
+        # 将 x-headers 放到 token 对象中，用以保存
+        if not self.token.x_device_id:
+            self.log.info('初始化 x_device_id')
+            self.token.x_device_id = self._x_device_id
+            self._save()
 
     def _save(self):
         """保存配置文件"""
         self.log.info(f'保存配置文件 {self._name}')
         json.dump(asdict(self.token), self._name.open('w', encoding='utf8'))
 
     # noinspection PyPep8Naming
@@ -219,14 +234,27 @@
 
         # 获取解析出来的 refreshToken, 使用这个token获取下载链接是直链, 不需要带 referer header
         refresh_token = json.loads(bizExt)['pds_login_result']['refreshToken']
         self._refresh_token(refresh_token, True)
 
     def _login_by_qrcode(self) -> requests.Response:
         """二维码登录"""
+        self.session.get(AUTH_HOST + V2_OAUTH_AUTHORIZE, params={
+            'login_type': 'custom',
+            'response_type': 'code',
+            'redirect_uri': 'https://www.aliyundrive.com/sign/callback',
+            'client_id': CLIENT_ID,
+            'state': r'{"origin":"file://"}',
+            # 'state': '{"origin":"https://www.aliyundrive.com"}',
+        }, stream=True).close()
+
+        #
+        session_id = self.session.cookies.get('SESSIONID')
+        self.log.debug(f'SESSIONID {session_id}')
+
         response = self.session.get(
             PASSPORT_HOST + NEWLOGIN_QRCODE_GENERATE_DO, params=UNI_PARAMS
         )
         self._log_response(response)
         data = response.json()['content']['data']
 
         qr_link = data['codeContent']
@@ -246,15 +274,14 @@
         self.log.info('等待扫描二维码')
 
         while True:
             response = self.session.post(
                 PASSPORT_HOST + NEWLOGIN_QRCODE_QUERY_DO,
                 data=data, params=UNI_PARAMS
             )
-            self._log_response(response)
             login_data = response.json()['content']['data']
             # noinspection PyPep8Naming
             qrCodeStatus = login_data['qrCodeStatus']
             # noinspection SpellCheckingInspection
             if qrCodeStatus == 'NEW':
                 pass
             elif qrCodeStatus == 'SCANED':
@@ -284,34 +311,42 @@
                 'refresh_token': refresh_token,
                 'grant_type': 'refresh_token'
             }
         )
         self._log_response(response)
         if response.status_code == 200:
             self.log.info('刷新 token 成功')
-            # noinspection PyProtectedMember
             self.token = DataClass.fill_attrs(Token, response.json())
-            self._save()
+            self.session.headers.update({
+                'Authorization': self.token.access_token,
+            })
+            if not self._x_device_id:
+                self._init_x_headers()
+            else:
+                self.token.x_device_id = self._x_device_id
+                self._save()
+        elif response.status_code == 502:
+            if loop_call:
+                self.log.warning('刷新 token 失败')
+                self.error_log_exit(response)
+            self.log.warning('刷新 token 时出现 502 网关错误，暂停10秒后重试')
+            time.sleep(10)
+            return self._refresh_token(refresh_token=refresh_token, loop_call=True)
         else:
             self.log.warning('刷新 token 失败')
             if loop_call:
                 # 从 _login 调用，则不继续调用 _login，防止循环调用
                 # 走到这里 说明 登录失败，则 退出
                 self.error_log_exit(response)
             else:
                 self.debug_log(response)
                 if self._re_login:
                     self._login()
                 else:
-                    raise AligoRefreshFailed('使用 refresh_token 刷新 token 失败，re_login=False，不继续（等待）登录')
-        self.session.headers.update({
-            'Authorization': self.token.access_token
-        })
-
-    _VERIFY_SSL = True
+                    raise AligoRefreshFailed('使用 refresh_token 刷新 token 失败，re_login=False，不继续登录')
 
     def request(self, method: str, url: str, params: Dict = None,
                 headers: Dict = None, data=None, body: Dict = None) -> requests.Response:
         """统一请求方法"""
         # 删除值为None的键
         if body is not None:
             body = {k: v for k, v in body.items() if v is not None}
@@ -331,46 +366,59 @@
                 time.sleep(self._request_failed_delay)
                 continue
 
             status_code = response.status_code
             self._log_response(response)
 
             if status_code == 401:
-                if 'ShareLinkToken' not in response.text:
-                    self._refresh_token()
-                else:
+                if b'"ShareLinkTokenInvalid"' in response.content:
                     # 刷新 share_token
                     share_id = body['share_id']
                     share_pwd = body['share_pwd']
                     r = self.post(
                         V2_SHARE_LINK_GET_SHARE_TOKEN,
-                        body={
-                            'share_id': share_id,
-                            'share_pwd': share_pwd
-                        }
+                        body={'share_id': share_id, 'share_pwd': share_pwd}
                     )
                     share_token = r.json()['share_token']
                     headers['x-share-token'].share_token = share_token
+                elif b'"UserDeviceOffline"' in response.content:
+                    self._create_session()
+                else:
+                    self._refresh_token()
                 continue
 
-            if status_code == 429:
+            if status_code in [429, 502, 504]:
                 if self._SLEEP_TIME_SEC is None:
                     sleep_int = 5 ** (i % 4)
                 else:
                     sleep_int = self._SLEEP_TIME_SEC
-                self.log.warning(f'请求太频繁，暂停 {sleep_int} 秒钟')
+                err_msg = None
+                if status_code == 429:
+                    err_msg = '请求太频繁'
+                elif status_code == 502:
+                    err_msg = '内部网关错误'
+                elif status_code == 504:
+                    err_msg = '内部网关超时'
+                self.log.warning(f'{err_msg}，暂停 {sleep_int} 秒钟')
                 time.sleep(sleep_int)
                 continue
 
             if status_code == 500:
                 raise AligoStatus500(response.content)
 
+            if status_code == 400:
+                if b'"DeviceSessionSignatureInvalid"' in response.content:
+                    self._create_session()
+                    continue
+                elif b'"InvalidResource.FileTypeFolder"' in response.content:
+                    self.log.warning(
+                        '请区分 文件 和 文件夹，有些操作是它们独有的，比如获取下载链接，很显然 文件夹 是没有的！')
             return response
 
-        self.log.info(f'重试 5 次仍旧失败')
+        self.log.info(f'重试 5 次仍失败，抛出异常')
         self.error_log_exit(response)
 
     def get(self, path: str, host: str = API_HOST, params: dict = None, headers: dict = None) -> requests.Response:
         """..."""
         return self.request(method='GET', url=host + path, params=params, headers=headers)
 
     def post(self, path: str, host: str = API_HOST, params: dict = None, headers: dict = None,
@@ -435,22 +483,21 @@
         """发送邮件"""
         qr_img = qrcode.make(qr_link)
         qr_img.get_image()
         qr_img_path = tempfile.mktemp()
         qr_img.save(qr_img_path)
         qr_data = open(qr_img_path, 'rb').read()
         send_email(
-            self._email[0], self._name_name, self._email[1], qr_data,
-            self._EMAIL_USER, self._EMAIL_PASSWORD, self._EMAIL_HOST, self._EMAIL_PORT
+            self._email.email, self._name_name, self._email.content, qr_data,
+            self._email.user, self._email.password, self._email.host, self._email.port
         )
         os.remove(qr_img_path)
-        self.log.info(f'登录二维码已发送至 {self._email[0]}')
+        self.log.info(f'登录二维码已发送至 {self._email.email}')
 
     def _log_response(self, response: requests.Response):
         """打印响应日志"""
         self.log.info(
             f'{response.request.method} {response.url} {response.status_code} {len(response.content)}'
         )
 
-    def logout(self):
-        """退出"""
-        self._name.unlink()
+    def device_logout(self):
+        return self.post(USERS_V1_USERS_DEVICE_LOGOUT)
```

### Comparing `aligo-5.5.9/aligo/core/BaseAligo.py` & `aligo-6.0.0/src/aligo/core/BaseAligo.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """..."""
 import json
 import logging
 import subprocess
 import traceback
 from dataclasses import asdict, is_dataclass
-from typing import Generic, List, Iterator, Dict, Callable, Union, Tuple, Type
+from typing import Generic, List, Iterator, Dict, Callable, Union, Type
 
 import requests
 
 from aligo.core import *
 from aligo.core.Config import *
 from aligo.request import *
 from aligo.response import *
@@ -25,32 +25,30 @@
             name: str = 'aligo',
             refresh_token: str = None,
             show: Callable[[str], None] = None,
             level: int = logging.DEBUG,
             use_aria2: bool = False,
             proxies: Dict = None,
             port: int = None,
-            email: Tuple[str, str] = None,
+            email: EMailConfig = None,
             request_failed_delay: float = 3,
             requests_timeout: float = None,
             login_timeout: float = None,
             re_login: bool = True
     ):
         """
         BaseAligo
         :param name: (可选, 默认: aligo) 配置文件名称, 便于使用不同配置文件进行身份验证
         :param refresh_token:
         :param show: (可选) 显示二维码的函数
         :param level: (可选) 控制控制台输出
         :param use_aria2: [bool] 是否使用 aria2 下载
         :param proxies: (可选) 自定义代理 [proxies={"https":"localhost:10809"}],支持 http 和 socks5（具体参考requests库的用法）
         :param port: (可选) 开启 http server 端口，用于网页端扫码登录. 提供此值时，将不再弹出或打印二维码
-        :param email: (可选) 发送扫码登录邮件 ("接收邮件的邮箱地址", "防伪字符串"). 提供此值时，将不再弹出或打印二维码
-            关于防伪字符串: 为了方便大家使用, aligo 自带公开邮箱, 省去邮箱配置的麻烦.
-                        所以收到登录邮件后, 一定要对比确认防伪字符串和你设置一致才可扫码登录, 否则将导致: 包括但不限于云盘文件泄露.
+        :param email: (可选) 邮箱配置，参考 EMailConfig
         :param request_failed_delay: 请求失败后，延迟时间，单位：秒
         :param requests_timeout: same as requests timeout
         :param login_timeout: 登录超时时间，单位：秒
         :param re_login: refresh_token 失效后是否继续登录（弹出二维码或邮件，需等待） fix #73
         """
         self._auth: Auth = Auth(  # type: ignore
             name=name,
@@ -86,27 +84,28 @@
 
     def _post(
             self,
             path: str,
             host: str = API_HOST,
             body: Union[DataType, Dict] = None,
             headers: dict = None,
-            ignore_auth: bool = False
+            ignore_auth: bool = False,
+            params: dict = None,
     ) -> requests.Response:
         """统一处理数据类型和 drive_id"""
         if body is None:
             body = {}
         elif isinstance(body, DataClass):
             body = asdict(body)
 
         if 'drive_id' in body and body['drive_id'] is None:
             # 如果存在 attr drive_id 并且它是 None，并将 default_drive_id 设置为它
             body['drive_id'] = self.default_drive_id
 
-        return self._auth.post(path=path, host=host, body=body, headers=headers, ignore_auth=ignore_auth)
+        return self._auth.post(path=path, host=host, body=body, headers=headers, ignore_auth=ignore_auth, params=params)
 
     @property
     def default_drive_id(self):
         """默认 drive_id"""
         return self._auth.token.default_drive_id
 
     @property
@@ -127,15 +126,15 @@
     @property
     def nick_name(self):
         """昵称"""
         return self._auth.token.nick_name
 
     def _result(self, response: requests.Response,
                 cls: Generic[DataType],
-                status_code: Union[List, int] = 200) -> Union[Null, DataType]:
+                status_code: Union[List, int] = 200, field: str = None) -> Union[Null, DataType]:
         """统一处理响应
 
         :param response:
         :param cls:
         :param status_code:
         :return:
         """
@@ -143,51 +142,57 @@
             status_code = [status_code]
         if response.status_code in status_code:
             text = response.text
             if not text.startswith('{'):
                 return cls()
             try:
                 # noinspection PyProtectedMember
-                return DataClass.fill_attrs(cls, json.loads(text))
+                d = json.loads(text)
+                if field:
+                    for i in field.split('.'):
+                        d = d[i]
+                if isinstance(d, list):
+                    return [DataClass.fill_attrs(cls, i) for i in d]
+                return DataClass.fill_attrs(cls, d)
             except TypeError:
                 self._auth.debug_log(response)
                 self._auth.log.error(cls)
                 traceback.print_exc()
         self._auth.log.warning(f'{response.status_code} {response.text[:200]}')
         return Null(response)
 
     def _list_file(
             self, path: str, body: Union[DataClass, Dict],
-            resp_type: Generic[DataType], headers: dict = None) -> Iterator[DataType]:
+            resp_type: Generic[DataType], headers: dict = None, params: dict = None) -> Iterator[DataType]:
         """
         枚举文件: 用于统一处理 1.文件列表 2.搜索文件列表 3.收藏列表 4.回收站列表
         :param path: [str] 批量处理的路径
         :param body: [DataClass] 批量处理的参数
         :param resp_type: [Callable] 响应类型
         :return: [Iterator[DataType]] 响应结果
 
         如何判断请求失败与否（适用于所有使用此方法的上层方法）：
         >>> from aligo import Aligo
         >>> ali = Aligo()
         >>> result = ali.get_file_list('<file_id>')
         >>> if isinstance(result[-1], Null):
         >>>     print('请求失败')
         """
-        response = self._post(path, body=body, headers=headers)
+        response = self._post(path, body=body, headers=headers, params=params)
         file_list = self._result(response, resp_type)
         if isinstance(file_list, Null):
             yield file_list
             return
         yield from file_list.items
         if file_list.next_marker != '':
             if isinstance(body, dict):
                 body['marker'] = file_list.next_marker
             else:
                 body.marker = file_list.next_marker
-            yield from self._list_file(path=path, body=body, resp_type=resp_type, headers=headers)
+            yield from self._list_file(path=path, body=body, resp_type=resp_type, headers=headers, params=params)
 
     def _core_get_file(self, body: GetFileRequest) -> BaseFile:
         """获取文件信息, 其他类中可能会用到, 所以放到基类中"""
         response = self._post(V2_FILE_GET, body=body)
         return self._result(response, BaseFile)
 
     def get_personal_info(self) -> GetPersonalInfoResponse:
@@ -251,11 +256,7 @@
                         # }
                         # status 409
                         i.body = DataClass.fill_attrs(body_type, i.body)
                     except TypeError:
                         # self._auth.log.warning(i)
                         pass
                 yield i
-
-    def logout(self):
-        """退出登录"""
-        self._auth.logout()
```

### Comparing `aligo-5.5.9/aligo/core/Compress.py` & `aligo-6.0.0/src/aligo/core/Compress.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/core/Config.py` & `aligo-6.0.0/src/aligo/core/Config.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 NEWLOGIN_QRCODE_GENERATE_DO = '/newlogin/qrcode/generate.do'
 V2_OAUTH_TOKEN_LOGIN = '/v2/oauth/token_login'
 V2_OAUTH_AUTHORIZE = '/v2/oauth/authorize'
 V2_ACCOUNT_TOKEN = '/v2/account/token'
 TOKEN_REFRESH = '/token/refresh'
 TOKEN_GET = '/token/get'
 USERS_V1_USERS_DEVICE_RENEW_SESSION = '/users/v1/users/device/renew_session'
+USERS_V1_USERS_DEVICE_LOGOUT = '/users/v1/users/device_logout'
+USERS_V1_USERS_DEVICE_CREATE_SESSION = '/users/v1/users/device/create_session'
+USERS_V2_USERS_DEVICE_LIST = '/users/v2/users/device_list'
 
 # 基本信息
 V2_USER_GET = '/v2/user/get'
 ADRIVE_V1_USER_CONFIG_GET = '/adrive/v1/user_config/get'
 V2_DRIVE_GET = '/v2/drive/get'
 V2_DRIVE_GET_DEFAULT_DRIVE = '/v2/drive/get_default_drive'
 V2_DRIVE_LIST_MY_DRIVES = '/v2/drive/list_my_drives'
@@ -44,23 +47,25 @@
 ADRIVE_V2_FILE_CREATE = '/adrive/v2/file/create'
 V2_FILE_CREATE_WITH_PROOF = '/v2/file/create_with_proof'
 ADRIVE_V2_FILE_CREATEWITHFOLDERS = '/adrive/v2/file/createWithFolders'
 V2_FILE_GET_UPLOAD_URL = '/v2/file/get_upload_url'
 ADRIVE_V1_FILE_DUPLICATE_LIST = '/adrive/v1/file/duplicateList'
 ADRIVE_V1_FILE_LISTTOCLEAN = '/adrive/v1/file/listToClean'
 V2_FILE_GET_OFFICE_PREVIEW_URL = '/v2/file/get_office_preview_url'
+ADRIVE_V1_FILE_GET_FOLDER_SIZE_INFO = '/adrive/v1/file/get_folder_size_info'
 
 # 相册
 ADRIVE_V1_USER_ALBUMS_INFO = '/adrive/v1/user/albums_info'
 ADRIVE_V1_ALBUMHOME_ALBUMLIST = '/adrive/v1/albumHome/albumList'
 ADRIVE_V1_ALBUM_DELETE = '/adrive/v1/album/delete'
 ADRIVE_V1_ALBUM_GET = '/adrive/v1/album/get'
 ADRIVE_V1_ALBUM_CREATE = '/adrive/v1/album/create'
 ADRIVE_V1_ALBUM_LIST_FILES = '/adrive/v1/album/list_files'
 ADRIVE_V1_ALBUM_UPDATE = '/adrive/v1/album/update'
+ADRIVE_V1_ALBUM_ADD_FILES = '/adrive/v1/album/add_files'
 
 V2_AIMS_SEARCH = '/v2/aims/search'
 
 V2_FILE_GET_DOWNLOAD_URL = '/v2/file/get_download_url'
 
 # 回收站
 V2_RECYCLEBIN_TRASH = '/v2/recyclebin/trash'
@@ -74,14 +79,16 @@
 ADRIVE_V2_SHARE_LINK_CREATE = '/adrive/v2/share_link/create'
 ADRIVE_V2_SHARE_LINK_CANCEL = '/adrive/v2/share_link/cancel'
 ADRIVE_V2_SHARE_LINK_GET_SHARE_BY_ANONYMOUS = '/adrive/v2/share_link/get_share_by_anonymous'
 V2_SHARE_LINK_GET_SHARE_TOKEN = '/v2/share_link/get_share_token'
 V2_FILE_GET_SHARE_LINK_DOWNLOAD_URL = '/v2/file/get_share_link_download_url'
 ADRIVE_V2_SHARE_LINK_EXTRACT_CODE = '/adrive/v2/share_link/extract_code'
 RECOMMEND_V1_SHARELINK_SEARCH = '/recommend/v1/shareLink/search'
+ADRIVE_V2_FILE_LIST_BY_SHARE = '/adrive/v2/file/list_by_share'
+ADRIVE_V2_FILE_GET_BY_SHARE = '/adrive/v2/file/get_by_share'
 
 # 批量操作
 V3_BATCH = '/v3/batch'
 ADRIVE_V2_BATCH = '/adrive/v2/batch'
 
 # 福利码
 V1_USERS_REWARDS = '/v1/users/rewards'
@@ -100,9 +107,12 @@
 V2_TEMPLATE_TEST = '/v2/template/test'
 
 # 参数
 CLIENT_ID = '25dzX3vbYqktVxyX'
 UNI_PARAMS = {'appName': 'aliyun_drive'}
 UNI_HEADERS = {
     'Referer': 'https://aliyundrive.com',
-    'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.114 Safari/537.36',
+    'User-Agent': ('Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) '
+                   'Chrome/91.0.4472.114 Safari/537.36'),
+    # 没有此请求头，list file 获取不到 download_url 字段，url 不支持断点续传
+    'x-canary': 'client=web,app=adrive,version=v4.1.0',
 }
```

### Comparing `aligo-5.5.9/aligo/core/Copy.py` & `aligo-6.0.0/src/aligo/core/Copy.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/core/Core.py` & `aligo-6.0.0/src/aligo/core/Core.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/core/Create.py` & `aligo-6.0.0/src/aligo/core/Create.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/core/Download.py` & `aligo-6.0.0/src/aligo/core/Download.py`

 * *Files 7% similar despite different names*

```diff
@@ -88,23 +88,30 @@
         try:
             progress_bar = None
             # noinspection PyProtectedMember
             with self._session.get(url, headers={
                 'Range': f'bytes={tmp_size}-',
                 'Referer': 'https://www.aliyundrive.com/',
             }, stream=True) as resp:
-                llen = int(resp.headers.get('content-length', 0))
-                if resp.headers.get('Accept-Ranges', None) != 'bytes':
-                    raise ValueError(f'无效下载链接或链接已过期 {resp.url}')
-                progress_bar = tqdm(total=llen + tmp_size, unit='B', unit_scale=True, colour='#31a8ff')
-                progress_bar.update(tmp_size)
-                with open(tmp_file, 'ab') as f:
-                    for content in resp.iter_content(chunk_size=Download._DOWNLOAD_CHUNK_SIZE):
-                        progress_bar.update(len(content))
-                        f.write(content)
+                total_size = int(resp.headers.get('content-length', 0))
+                accept_range = resp.headers.get('Accept-Ranges', None)
+                if accept_range == 'bytes':
+                    progress_bar = tqdm(total=total_size + tmp_size, unit='B', unit_scale=True, colour='#31a8ff')
+                    progress_bar.update(tmp_size)
+                    with open(tmp_file, 'ab') as f:
+                        for content in resp.iter_content(chunk_size=Download._DOWNLOAD_CHUNK_SIZE):
+                            progress_bar.update(len(content))
+                            f.write(content)
+                else:
+                    self._auth.log.warning(f'不支持断点续传 {file_path}')
+                    progress_bar = tqdm(total=total_size, unit='B', unit_scale=True, colour='#31a8ff')
+                    with open(tmp_file, 'wb') as f:
+                        for content in resp.iter_content(chunk_size=Download._DOWNLOAD_CHUNK_SIZE):
+                            progress_bar.update(len(content))
+                            f.write(content)
             os.renames(tmp_file, file_path)
         finally:
             if progress_bar:
                 progress_bar.close()
 
         self._auth.log.info(f'文件下载完成 {file_path}')
         return file_path
@@ -122,14 +129,10 @@
         >>> # noinspection PyShadowingNames
         >>> file_path = ali.download_files([ali.get_file_by_path('xxx.mp3')])
         >>> print(file_path)
         """
         rt = []
         for file in files:
             file_path = os.path.join(local_folder, file.name)
-            try:
-                file_path = self._core_download_file(file_path, file.download_url)
-            except ValueError:
-                file = self._core_get_file(GetFileRequest(file_id=file.file_id, drive_id=file.drive_id))
-                file_path = self._core_download_file(file_path, file.download_url)
+            file_path = self._core_download_file(file_path, file.download_url or file.url)
             rt.append(file_path)
         return rt
```

### Comparing `aligo-5.5.9/aligo/core/Drive.py` & `aligo-6.0.0/src/aligo/core/Drive.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/core/Duplicate.py` & `aligo-6.0.0/src/aligo/core/Duplicate.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/core/EMail.py` & `aligo-6.0.0/src/aligo/core/EMail.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """发送邮件模块"""
 import smtplib
+import ssl
 import time
 from email.mime.image import MIMEImage
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
 from email.utils import formataddr
 
 
@@ -21,15 +22,18 @@
         MIMEText(f'<div align="center"><h3>{content}</h3><img style="max-width: 100%" src="cid:qrcode"></div>', 'html'))
 
     msg_image = MIMEImage(qr_data, 'png')
     msg_image.add_header('Content-ID', '<qrcode>')
 
     msg_root.attach(msg_image)
 
-    smtp = smtplib.SMTP_SSL(email_host, email_port)
+    try:
+        smtp = smtplib.SMTP_SSL(email_host, email_port)
+    except ssl.SSLError:
+        smtp = smtplib.SMTP(email_host, email_port)
     smtp.login(email_user, email_password)
     for i in range(1, 4):
         try:
             result = smtp.sendmail(
                 email_user,
                 [receiver],
                 msg_root.as_bytes()
```

### Comparing `aligo-5.5.9/aligo/core/File.py` & `aligo-6.0.0/src/aligo/core/Move.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 """..."""
 from typing import Iterator
 
 from aligo.core import *
 from aligo.core.Config import *
 from aligo.request import *
 from aligo.response import *
-from aligo.types import *
 
 
-class File(BaseAligo):
+class Move(BaseAligo):
     """..."""
 
-    def _core_get_file_list(self, body: GetFileListRequest) -> Iterator[BaseFile]:
+    def _core_move_file(self, body: MoveFileRequest) -> MoveFileResponse:
         """..."""
-        yield from self._list_file(ADRIVE_V3_FILE_LIST, body, GetFileListResponse)
+        response = self._post(V2_FILE_MOVE, body=body)
+        return self._result(response, MoveFileResponse)
 
-    def _core_batch_get_files(self, body: BatchGetFileRequest) -> Iterator[BatchSubResponse]:
-        """batch_get_files"""
+    def _core_batch_move_files(self, body: BatchMoveFilesRequest) -> Iterator[BatchSubResponse[MoveFileResponse]]:
+        """..."""
         if body.drive_id is None:
             body.drive_id = self.default_drive_id
 
         yield from self.batch_request(BatchRequest(
             requests=[BatchSubRequest(
                 id=file_id,
-                url='/file/get',
-                body=GetFileRequest(
-                    drive_id=body.drive_id, file_id=file_id
+                url='/file/move',
+                body=MoveFileRequest(
+                    drive_id=body.drive_id, file_id=file_id,
+                    to_parent_file_id=body.to_parent_file_id,
+                    overwrite=body.overwrite, auto_rename=body.auto_rename
                 )
             ) for file_id in body.file_id_list]
-        ), GetFileRequest)
+        ), MoveFileResponse)
```

### Comparing `aligo-5.5.9/aligo/core/LoginServer.py` & `aligo-6.0.0/src/aligo/core/LoginServer.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/core/Move.py` & `aligo-6.0.0/src/aligo/core/Update.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 """..."""
-from typing import Iterator
+
+from dataclasses import asdict
 
 from aligo.core import *
 from aligo.core.Config import *
 from aligo.request import *
-from aligo.response import *
+from aligo.types import *
 
 
-class Move(BaseAligo):
+class Update(BaseAligo):
     """..."""
 
-    def _core_move_file(self, body: MoveFileRequest) -> MoveFileResponse:
-        """..."""
-        response = self._post(V2_FILE_MOVE, body=body)
-        return self._result(response, MoveFileResponse)
+    def update_file(self, body: UpdateFileRequest) -> BaseFile:
+        """
+        Update file.
+        :param body: [UpdateFileRequest]
+        :return: [BaseFile]
+
+        :Example:
+        >>> from aligo import Aligo
+        >>> ali = Aligo()
+        >>> new_file = ali.update_file(UpdateFileRequest(file_id='file_id', name='new_name'))
+        >>> print(new_file.name)
+        """
+        response = self._post(V3_FILE_UPDATE, body=body)
+        return self._result(response, BaseFile)
 
-    def _core_batch_move_files(self, body: BatchMoveFilesRequest) -> Iterator[BatchSubResponse[MoveFileResponse]]:
+    def _core_rename_file(self, body: RenameFileRequest) -> BaseFile:
         """..."""
-        if body.drive_id is None:
-            body.drive_id = self.default_drive_id
-
-        yield from self.batch_request(BatchRequest(
-            requests=[BatchSubRequest(
-                id=file_id,
-                url='/file/move',
-                body=MoveFileRequest(
-                    drive_id=body.drive_id, file_id=file_id,
-                    to_parent_file_id=body.to_parent_file_id,
-                    overwrite=body.overwrite, auto_rename=body.auto_rename
-                )
-            ) for file_id in body.file_id_list]
-        ), MoveFileResponse)
+        return self.update_file(UpdateFileRequest(**asdict(body)))
```

### Comparing `aligo-5.5.9/aligo/core/Recyclebin.py` & `aligo-6.0.0/src/aligo/core/Recyclebin.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/core/Search.py` & `aligo-6.0.0/src/aligo/core/Search.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/core/Share.py` & `aligo-6.0.0/src/aligo/core/Share.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,20 +8,19 @@
 from aligo.response import *
 from aligo.types import *
 
 
 class Share(BaseAligo):
     """分享相关"""
 
-    def share_link_extract_code(self, content: str):
+    def share_link_extract_code(self, content: str) -> ShareLinkExtractCodeResponse:
         response = self._post(ADRIVE_V2_SHARE_LINK_EXTRACT_CODE, body={
             'content': content
         })
-        data = response.json()['data']
-        return DataClass.fill_attrs(ShareLinkExtractCodeResponse, data)
+        return self._result(response, ShareLinkExtractCodeResponse, field='data')
 
     def _core_share_file(self, body: CreateShareLinkRequest) -> CreateShareLinkResponse:
         """分享文件, 支持批量分享
 
         目前(2021年07月17日)官方只开放分享部分类型文件
         """
         response = self._post(ADRIVE_V2_SHARE_LINK_CREATE, body=body)
@@ -86,25 +85,54 @@
             yield file_list
             return
         yield from file_list.items
         if file_list.next_marker != '':
             body.marker = file_list.next_marker
             yield from self._core_get_share_file_list(body=body, x_share_token=x_share_token)
 
+    def _core_list_by_share(
+            self,
+            body: GetShareFileListRequest,
+            x_share_token: GetShareTokenResponse
+    ) -> Iterator[BaseShareFile]:
+        """..."""
+        response = self._auth.post(ADRIVE_V2_FILE_LIST_BY_SHARE, body=asdict(body),
+                                   headers={'x-share-token': x_share_token}, ignore_auth=True)
+        file_list = self._result(response, GetShareFileListResponse)
+        if isinstance(file_list, Null):
+            yield file_list
+            return
+        yield from file_list.items
+        if file_list.next_marker != '':
+            body.marker = file_list.next_marker
+            yield from self._core_list_by_share(body=body, x_share_token=x_share_token)
+
     def _core_get_share_file(
             self,
             body: GetShareFileRequest,
             x_share_token: GetShareTokenResponse
     ) -> BaseShareFile:
         """..."""
         response = self._auth.post(V2_FILE_GET, body=asdict(body), headers={'x-share-token': x_share_token},
                                    ignore_auth=True)
         share_file = self._result(response, BaseShareFile)
         return share_file
 
+    def _core_get_by_share(
+            self,
+            body: GetShareFileRequest,
+            x_share_token: GetShareTokenResponse
+    ) -> BaseShareFile:
+        """..."""
+        response = self._auth.post(ADRIVE_V2_FILE_GET_BY_SHARE, body=asdict(body),
+                                   headers={'x-share-token': x_share_token},
+                                   ignore_auth=True)
+        share_file = self._result(response, BaseShareFile)
+        return share_file
+
     def _core_get_share_link_download_url(
             self,
             body: GetShareLinkDownloadUrlRequest,
             x_share_token: GetShareTokenResponse
     ) -> GetShareLinkDownloadUrlResponse:
         """..."""
         response = self._auth.post(
```

### Comparing `aligo-5.5.9/aligo/core/Star.py` & `aligo-6.0.0/src/aligo/core/Star.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/core/User.py` & `aligo-6.0.0/src/aligo/core/User.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """..."""
 
+from typing import List
+
 from aligo.core import *
 from aligo.core.Config import *
 from aligo.response import RewardSpaceResponse, UsersVipInfoResponse
 from aligo.types import *
 
 
 class User(BaseAligo):
@@ -43,7 +45,11 @@
         response = self._post(ADRIVE_V1_USER_CONFIG_GET, body={})
         return self._result(response, UserConfig)
 
     def get_vip_info(self) -> UsersVipInfoResponse:
         """获取用户vip信息"""
         response = self._post(BUSINESS_V1_USERS_VIP_INFO, body={})
         return self._result(response, UsersVipInfoResponse)
+
+    def list_login_device(self) -> List[LoginDevice]:
+        response = self._post(USERS_V2_USERS_DEVICE_LIST)
+        return self._result(response, LoginDevice, field='result.devices')
```

### Comparing `aligo-5.5.9/aligo/core/Video.py` & `aligo-6.0.0/src/aligo/core/Video.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/request/AlbumListFilesRequest.py` & `aligo-6.0.0/src/aligo/request/AlbumListFilesRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/request/CreateFileRequest.py` & `aligo-6.0.0/src/aligo/request/CreateFileRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/request/CreateShareLinkRequest.py` & `aligo-6.0.0/src/aligo/request/CreateShareLinkRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/request/GetFileListRequest.py` & `aligo-6.0.0/src/aligo/request/GetFileListRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/request/GetFileRequest.py` & `aligo-6.0.0/src/aligo/request/GetFileRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/request/GetRecycleBinListRequest.py` & `aligo-6.0.0/src/aligo/request/GetRecycleBinListRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/request/GetShareFileListRequest.py` & `aligo-6.0.0/src/aligo/request/GetShareFileListRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/request/GetShareLinkDownloadUrlRequest.py` & `aligo-6.0.0/src/aligo/request/GetShareLinkDownloadUrlRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/request/GetShareLinkListRequest.py` & `aligo-6.0.0/src/aligo/request/GetShareLinkListRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/request/GetStarredListRequest.py` & `aligo-6.0.0/src/aligo/request/GetStarredListRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/request/SearchFileRequest.py` & `aligo-6.0.0/src/aligo/request/SearchFileRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/request/UpdateFileRequest.py` & `aligo-6.0.0/src/aligo/request/UpdateFileRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/request/UpdateShareLinkRequest.py` & `aligo-6.0.0/src/aligo/request/UpdateShareLinkRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/request/__init__.py` & `aligo-6.0.0/src/aligo/request/__init__.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/response/CreateFileResponse.py` & `aligo-6.0.0/src/aligo/response/CreateFileResponse.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/response/CreateShareLinkResponse.py` & `aligo-6.0.0/src/aligo/response/CreateShareLinkResponse.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/response/DuplicateListResponse.py` & `aligo-6.0.0/src/aligo/response/DuplicateListResponse.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/response/GetShareInfoResponse.py` & `aligo-6.0.0/src/aligo/response/GetShareInfoResponse.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/response/GetShareTokenResponse.py` & `aligo-6.0.0/src/aligo/response/GetShareTokenResponse.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/response/UpdateShareLinkResponse.py` & `aligo-6.0.0/src/aligo/response/UpdateShareLinkResponse.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/response/__init__.py` & `aligo-6.0.0/src/aligo/response/__init__.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/types/BaseAlbum.py` & `aligo-6.0.0/src/aligo/types/BaseAlbum.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/types/BaseDrive.py` & `aligo-6.0.0/src/aligo/types/BaseDrive.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/types/BaseFile.py` & `aligo-6.0.0/src/aligo/types/BaseFile.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/types/BaseShareFile.py` & `aligo-6.0.0/src/aligo/types/BaseShareFile.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,7 +41,8 @@
     drive_id: str = None
     domain_id: str = None
     revision_id: str = None
     # 2022年11月21日13时25分58秒
     starred: bool = False
     content_hash: str = None
     trashed_at: str = None
+    from_share_id : str = None
```

### Comparing `aligo-5.5.9/aligo/types/BaseUser.py` & `aligo-6.0.0/src/aligo/types/BaseUser.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/types/DataClass.py` & `aligo-6.0.0/src/aligo/types/DataClass.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,19 @@
 
 import logging
 import os
 from dataclasses import dataclass, is_dataclass
 from typing import TypeVar, Generic, Optional, List, Dict, Type
 
 import coloredlogs
-from typing_extensions import get_type_hints, get_origin, get_args
+
+try:
+    from typing import get_type_hints, get_origin, get_args
+except ImportError:
+    from typing_extensions import get_type_hints, get_origin, get_args
 
 DataType = TypeVar('DataType')
 
 _HINTS = {}
 _LOGGER = logging.getLogger(__name__)
 _ALIGO_DEBUG = os.getenv('ALIGO_DEBUG')
```

### Comparing `aligo-5.5.9/aligo/types/Enum.py` & `aligo-6.0.0/src/aligo/types/Enum.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 """字面量值"""
 from typing import Optional
 
-from typing_extensions import Literal
+try:
+    from typing import Literal
+except ImportError:
+    from typing_extensions import Literal
 
 MediaTranscodeStatus = Optional[
     # 媒体转码状态
     Literal[
         'running',  # 转码中
         'finished',  # 转码完成
         'failed',  # 转码失败
```

### Comparing `aligo-5.5.9/aligo/types/ImageMedia.py` & `aligo-6.0.0/src/aligo/types/ImageMedia.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/types/ShareLinkSchema.py` & `aligo-6.0.0/src/aligo/types/ShareLinkSchema.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/types/Token.py` & `aligo-6.0.0/src/aligo/types/Token.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,7 +28,9 @@
     pin_setup: bool = field(default=None, repr=False)
     is_first_login: bool = field(default=None, repr=False)
     need_rp_verify: bool = field(default=None, repr=False)
     device_id: str = field(default=None, repr=False)
     domain_id: str = field(default=None, repr=False)
     # noinspection SpellCheckingInspection
     hlogin_url: str = field(default=None, repr=False)
+    # x-signature x-device-id x-nonce
+    x_device_id: str = field(default=None, repr=False)
```

### Comparing `aligo-5.5.9/aligo/types/UserConfig.py` & `aligo-6.0.0/src/aligo/types/UserConfig.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/types/VideoMedia.py` & `aligo-6.0.0/src/aligo/types/VideoMedia.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/types/VideoPreview.py` & `aligo-6.0.0/src/aligo/types/VideoPreview.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/types/VideoPreviewPlayInfo.py` & `aligo-6.0.0/src/aligo/types/VideoPreviewPlayInfo.py`

 * *Files identical despite different names*

### Comparing `aligo-5.5.9/aligo/types/__init__.py` & `aligo-6.0.0/src/aligo/types/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,19 +10,22 @@
 from .BaseFile import BaseFile
 from .BaseShareFile import BaseShareFile
 from .BaseUser import BaseUser
 from .CroppingBoundary import CroppingBoundary
 from .CroppingSuggestionItem import CroppingSuggestionItem
 from .DataClass import DataClass
 from .DriveCapacityDetail import DriveCapacityDetail
+from .EMailConfig import EMailConfig
 from .FaceThumbnail import FaceThumbnail
+from .FolderSizeInfo import FolderSizeInfo
 from .ImageMedia import ImageMedia
 from .ImageQuality import ImageQuality
 from .ImageTag import ImageTag
 from .ListAlbumItem import ListAlbumItem
+from .LoginDevice import LoginDevice
 from .LoginTimout import LoginTimeout
 from .MediaTransCodeTemplate import MediaTransCodeTemplate
 from .Null import Null
 from .PersonalRightsInfo import PersonalRightsInfo
 from .PersonalSpaceInfo import PersonalSpaceInfo
 from .Privilege import Privilege
 from .RateLimit import RateLimit
```

### Comparing `aligo-5.5.9/aligo.egg-info/PKG-INFO` & `aligo-6.0.0/src/aligo.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,170 +1,197 @@
 Metadata-Version: 2.1
 Name: aligo
-Version: 5.5.9
-Summary: aliyundrive apis package
-Home-page: https://github.com/foyoux/aligo
-Author: foyou
-Author-email: yimi.0822@qq.com
-License: GPL-3.0
+Version: 6.0.0
+Summary: aliyun drive sdk
+Author: foyoux
 Project-URL: Source, https://github.com/foyoux/aligo
+Project-URL: Homepage, https://github.com/foyoux/aligo
 Project-URL: Bug Tracker, https://github.com/foyoux/aligo/issues
-Description: # aligo
-        
-        🚀🔥 简单、易用、可扩展的阿里云盘 API 接口库 👍👍
-        
-        [wiki 文档](https://github.com/foyoux/aligo/wiki) + [examples](https://github.com/foyoux/aligo/tree/main/examples)
-        
-        > 文档写得很简单，详情请查看 代码提示 + 文档注释
-        > 
-        > 有任何疑问 请 [issue](https://github.com/foyoux/aligo/issues/new?assignees=&labels=&template=bug_report.md&title=)
-        > 或 加入 **aligo交流反馈群** （群二维码在底部）
-        
-        [![python version](https://img.shields.io/pypi/pyversions/aligo)](https://pypi.org/project/aligo/)  [![Downloads](https://static.pepy.tech/personalized-badge/aligo?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/aligo)
-        
-        ```bash
-        pip install --upgrade aligo
-        ```
-        
-        ## 快速入门
-        
-        ```python
-        """快速入门"""
-        from aligo import Aligo
-        
-        if __name__ == '__main__':
-            ali = Aligo()  # 第一次使用，会弹出二维码，供扫描登录
-            
-            user = ali.get_user()  # 获取用户信息
-            print(user.user_name, user.nick_name, user.phone)  # 打印用户信息
-            
-            ll = ali.get_file_list()  # 获取网盘根目录文件列表
-            for file in ll:  # 遍历文件列表
-                print(file.file_id, file.name, file.type)  # 打印文件信息
-        ```
-        
-        https://user-images.githubusercontent.com/35125624/150529002-c2f1b80b-fb11-4e0a-9fd7-6f57f678ccf5.mp4
-        
-        ## 基本功能
-        
-        - [x] 完全的代码提示
-        - [x] 持久化登录、多帐户登录
-        - [x] 福利码兑换
-        - [x] 文件夹同步
-        - [x] 在线解压缩
-        - [x] 支持功能扩展
-        - [x] 搜索文件/标签
-        - [x] 获取重复文件列表
-        - [x] 文件（夹）重命名
-        - [x] 文件（夹）上传下载
-        - [x] 文件（夹）移动复制
-        - [x] 文件（夹）删除恢复
-        - [x] 获取文档在线预览接口
-        - [x] 文件（夹）分享 保存 收藏
-        - [x] 文件（夹）自定义分享（无限制）
-        - [x] 获取帐户、云盘（容量）等基本信息
-        - [x] 相册 创建 删除 修改 添加文件 获取文件
-        - [x] 。。。。。。
-        - [x] ⭐⭐⭐ 欢迎大家发起 [新功能请求](https://github.com/foyoux/aligo/issues/new?assignees=&labels=&template=feature_request.md&title=)
-        
-        > **温馨提示：**
-        >   1. 由于秒传链接的失效，自定分享信息的有效期只有4个小时。
-        >   2. 阿里云盘不同于其他网盘或系统，其定位文件不是基于文件名（路径），而是通过 `file_id`，这才是唯一定位文件的方式，**aligo** 中提供了简便函数 `get_file_by_path`/`get_folder_by_path`，通过网盘路径获取文件对象，通过 其上的 `file_id` 属性即可获取所需文件标识。但不建议频繁使用此方法，因为内部是通过 `get_file_list` 遍历得到的。
-        >   3. 在保存超大分享时（分享中的文件特别多），执行保存全部的方法 - `share_file_save_all_to_drive`，它会立刻执行完毕，但是文件不会立刻被保存到网盘中，阿里云盘服务器会帮你在后台陆续将所有文件存到你的网盘中；所有当你使用 `share_file_save_all_to_drive` 保存超大分享时，却只看到一部分文件时，不用疑惑，这是正常情况。
-        
-        
-        ## 网页扫码登录
-        
-        ```python
-        
-        from aligo import Aligo
-        
-        # 提供 port 参数即可, 之后打开浏览器访问 http://<YOUR_IP>:<port>
-        ali = Aligo(port=8080)
-        ```
-        
-        
-        ## 发送登录二维码到邮箱（推荐）
-        **最佳实践**：建议将邮箱绑定到微信，这样能实时收到提醒，登录过期后也可以第一时间收到登录请求。
-        
-        **安全性问题**：虽然自带公开邮箱（任何人都可以通过此邮箱向你发邮件），但是他人并不能通过这个获取任何人发送的邮件，所以 防伪字符串 策略是安全的。
-        
-        ```python
-        
-        from aligo import Aligo
-        
-        
-        """
-        email: 发送扫码登录邮件 ("接收邮件的邮箱地址", "防伪字符串"). 提供此值时，将不再弹出或打印二维码
-                关于防伪字符串: 为了方便大家使用, aligo 自带公开邮箱, 省去邮箱配置的麻烦.
-                所以收到登录邮件后, 一定要对比确认防伪字符串和你设置一致才可扫码登录, 否则将导致: 包括但不限于云盘文件泄露.
-        """
-        
-        # 提供 email 参数即可
-        ali = Aligo(email=('xxx@qq.com', '防伪字符串，可任意字符串'))
-        ```
-        
-        ## 如何彻底删除文件？
-        > 无需先移动文件到回收站
-        
-        此功能太危险，**aligo** 未直接提供。不过 [这里](https://github.com/foyoux/aligo/wiki/%E8%87%AA%E5%AE%9A%E4%B9%89%E5%8A%9F%E8%83%BD---%E5%BD%BB%E5%BA%95%E5%88%A0%E9%99%A4%E6%96%87%E4%BB%B6) 扩展了该功能，请小心使用！
-        
-        
-        ## 关于扩展功能
-        
-        一般步骤：
-        
-            1. 使用浏览器或其他抓包工具，观察通信过程；
-            2. 获取 url/path + 请求体；
-            3. 继承 `Aligo`, 使用现有的方法 `self._post` 等，进行发送请求；
-            
-        会自动维护 **token**, 你只需关注如何发送请求即可
-        
-        [扩展功能举栗🌰 - 配有视频和代码](https://github.com/foyoux/aligo/issues/24)
-        
-        
-        ## 不慎泄露 refresh_token ?
-        
-        必须马上修改密码！必须马上修改密码！必须马上修改密码！
-        
-        
-        ## 声明
-        
-        此项目仅供学习交流，若有不妥之处，侵联必删。
-        
-        此项目仅供学习交流，若有不妥之处，侵联必删。
-        
-        此项目仅供学习交流，若有不妥之处，侵联必删。
-        
-        ---
-        
-        <table align="center">
-            <thead align="center">
-            <tr>
-                <td><h2>❤️‍🔥欢迎加入🤝🏼</h2></td>
-            </tr>
-            </thead>
-            <tbody align="center">
-            <tr>
-                <td><img src="http://110.42.175.98:5512/down/LKPvT9xK2lFx?fname=/aligo/wechat.jpg" alt="aligo反馈交流群"/></td>
-            </tr>
-            </tbody>
-            <tfoot align="center">
-            <tr>
-                <td>😃 二维码会保持更新 😜</td>
-            </tr>
-            </tfoot>
-        </table>
-Keywords: aligo aliyun drive aliyundrive cloud pcs aliyunpan
-Platform: UNKNOWN
+Keywords: aligo
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Environment :: Console
-Classifier: Natural Language :: Chinese (Simplified)
-Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.7.*
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# aligo
+
+🚀🔥 简单、易用、可扩展的阿里云盘 API 接口库 👍👍
+
+[wiki 文档](https://github.com/foyoux/aligo/wiki) + [examples](https://github.com/foyoux/aligo/tree/main/examples)
+
+> 文档写得很简单，详情请查看 代码提示 + 文档注释
+> 
+> 有任何疑问 请 [issue](https://github.com/foyoux/aligo/issues/new?assignees=&labels=&template=bug_report.md&title=)
+> 或 加入 **aligo交流反馈群** （群二维码在底部）
+
+[![python version](https://img.shields.io/pypi/pyversions/aligo)](https://pypi.org/project/aligo/)  [![Downloads](https://static.pepy.tech/personalized-badge/aligo?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/aligo)
+
+```sh
+pip install -U aligo
+pip install git+https://github.com/foyoux/aligo.git
+```
+
+## 快速入门
+
+```python
+"""快速入门"""
+from aligo import Aligo
+
+if __name__ == '__main__':
+    ali = Aligo()  # 第一次使用，会弹出二维码，供扫描登录
+    
+    user = ali.get_user()  # 获取用户信息
+    print(user.user_name, user.nick_name, user.phone)  # 打印用户信息
+    
+    ll = ali.get_file_list()  # 获取网盘根目录文件列表
+    for file in ll:  # 遍历文件列表
+        print(file.file_id, file.name, file.type)  # 打印文件信息
+```
+
+https://user-images.githubusercontent.com/35125624/150529002-c2f1b80b-fb11-4e0a-9fd7-6f57f678ccf5.mp4
+
+## 基本功能
+
+- [x] 完全的代码提示
+- [x] 持久化登录、多帐户登录
+- [x] 福利码兑换
+- [x] 文件夹同步
+- [x] 在线解压缩
+- [x] 支持功能扩展
+- [x] 搜索文件/标签
+- [x] 获取重复文件列表
+- [x] 文件（夹）重命名
+- [x] 文件（夹）上传下载
+- [x] 文件（夹）移动复制
+- [x] 文件（夹）删除恢复
+- [x] 获取文档在线预览接口
+- [x] 文件（夹）分享 保存 收藏
+- [x] 文件（夹）自定义分享（无限制）
+- [x] 获取帐户、云盘（容量）等基本信息
+- [x] 相册 创建 删除 修改 添加文件 获取文件
+
+更多接口功能，请安装最新版尝试
+
+欢迎大家发起 [新功能请求](https://github.com/foyoux/aligo/issues/new?assignees=&labels=&template=feature_request.md&title=)
+
+> **温馨提示：**
+>   1. 由于秒传链接的失效，自定分享信息的有效期只有4个小时。
+>   2. 阿里云盘不同于其他网盘或系统，其定位文件不是基于文件名（路径），而是通过 `file_id`，这才是唯一定位文件的方式，**aligo** 中提供了简便函数 `get_file_by_path`/`get_folder_by_path`，通过网盘路径获取文件对象，通过 其上的 `file_id` 属性即可获取所需文件标识。但不建议频繁使用此方法，因为内部是通过 `get_file_list` 遍历得到的。
+>   3. 在保存超大分享时（分享中的文件特别多），执行保存全部的方法 - `share_file_save_all_to_drive`，它会立刻执行完毕，但是文件不会立刻被保存到网盘中，阿里云盘服务器会帮你在后台陆续将所有文件存到你的网盘中；所有当你使用 `share_file_save_all_to_drive` 保存超大分享时，却只看到一部分文件时，不用疑惑，这是正常情况。
+
+## 登录
+### 网页扫码登录
+
+```python
+from aligo import Aligo
+
+# 提供 port 参数即可, 之后打开浏览器访问 http://<YOUR_IP>:<port>
+ali = Aligo(port=8080)
+```
+
+
+### 发送登录二维码到邮箱（推荐）
+
+**最佳实践**：建议将邮箱绑定到微信，这样能实时收到提醒，登录过期后也可以第一时间收到登录请求。
+
+```python
+from aligo import Aligo, EMailConfig
+
+if __name__ == '__main__':
+    email_config = EMailConfig(
+        email='<接收登录邮件的邮箱地址>',
+        # 自配邮箱
+        user='',
+        password='',
+        host='',
+        port=0,
+    )
+    ali = Aligo(email=email_config)
+```
+
+## 文件夹同步
+文件夹同步有三种不同的方法，但都可以通过flag参数设置，注意区分。
+```python
+from aligo import Aligo
+
+"""
+flag: 同步标志（类型），默认：None, 另外可选：True, False
+        None：双端同步
+        True：以本地为主
+        False：以云端为主
+"""
+
+ali = Aligo()
+local_folder = 'Path of local'
+remote_id = 'remote id'
+ali.sync_folder(local_folder=local_folder, remote_folder=remote_id,flag=True) 
+```
+
+## 文件上传/下载
+文件的上传与下载有多种不同的实现方法，具体使用请阅读源代码。
+```python
+from aligo import Aligo
+ali = Aligo()
+ali.upload_files(file_paths='file_names' , parent_file_id='reading_id')
+ali.download_file(file_id='<file_id>')
+```
+
+
+## 如何彻底删除文件？
+> 无需先移动文件到回收站
+
+此功能太危险，**aligo** 未直接提供。不过 [这里](https://github.com/foyoux/aligo/wiki/%E8%87%AA%E5%AE%9A%E4%B9%89%E5%8A%9F%E8%83%BD---%E5%BD%BB%E5%BA%95%E5%88%A0%E9%99%A4%E6%96%87%E4%BB%B6) 扩展了该功能，请小心使用！
+
+
+## 关于扩展功能
+
+一般步骤：
+
+    1. 使用浏览器或其他抓包工具，观察通信过程；
+    2. 获取 url/path + 请求体；
+    3. 继承 `Aligo`, 使用现有的方法 `self._post` 等，进行发送请求；
+    
+会自动维护 **token**, 你只需关注如何发送请求即可
+
+[扩展功能举栗🌰 - 配有视频和代码](https://github.com/foyoux/aligo/issues/24)
+
+
+## 不慎泄露 refresh_token ?
+
+虽然官方提供下线功能，但还是要 马上修改密码
+
+今天无意中发现，之前使用 aligo 登录的会在登录设备列表中，但今天发现再使用 aligo 登录，已经不会出现在登录设备列表中，我也不知道为什么
+
+今天把除我手机之外的所有设备下线后，包括 Chrome 和 aligo 登录的，但并没有失效，所有的 token 和 refresh_token 还是可以使用
+
+所以还是得 -> 必须马上修改密码！必须马上修改密码！必须马上修改密码！
+
+
+## 声明
+
+此项目仅供学习交流，若有不妥之处，侵联必删。
+
+---
+
+<table align="center">
+    <thead align="center">
+    <tr>
+        <td><h2>❤️‍🔥欢迎加入🤝🏼</h2></td>
+    </tr>
+    </thead>
+    <tbody align="center">
+    <tr>
+        <td><img src="http://110.42.175.98:5512/down/LKPvT9xK2lFx?fname=/aligo/wechat.jpg" alt="aligo反馈交流群"/></td>
+    </tr>
+    </tbody>
+    <tfoot align="center">
+    <tr>
+        <td>😃 二维码会保持更新 😜</td>
+    </tr>
+    </tfoot>
+</table>
```

