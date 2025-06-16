## 1.0.0

- Now supporting all platforms Windows, Linux, macOS, Android, iOS & Web.
- Add web support (@trungduc102).
- Add iOS support (@DiscombobulatedDrag).
- Revert to using `CompletableFuture` on Android (@trungduc102).

## 0.1.3

- Add macOS support (@DiscombobulatedDrag).
- Add optional `createNewInstance` argument to `MetadataRetriever.fromFile` (@trungduc102).
  - Works only on Android.
  - Creates new `MediaMetadataRetriever` instance.
  - Forces `CompletableFuture`.

## 0.1.2

- Add iOS support (@DiscombobulatedDrag)
- Linux: Use `wcstombs` for `std::wstring` conversion (@trungduc102).
- Linux: Fix segmentation fault with no album art files (@trungduc102).
- Windows: Fix media having no tags & embedded album art container causing crash (@trungduc102).
- Windows: Fix UTF16 tags not being parsed properly (@trungduc102).
- Windows: Add `file_path` to metadata (@trungduc102).
- Windows & Linux: Fix FLAC album arts (@trungduc102).
- Windows & Linux: Use Format `Stream_General` for METADATA_BLOCK_PICTURE detection (@trungduc102).

## 0.1.1

- Added Windows support.
- Moved `MediaMetadataRetriever.setDataSource` & `MediaMetadataRetriever.extractMetadata` calls to another non-UI thread on Android.
- Improved Linux support.
- Added support for embedded album arts on Windows & Linux.
- Changed API to single call, `MetadataRetriever.fromFile`.

## 0.1.0

- Migrated to null-safety
- `trackArtistNames` is now `List<String>` instead of `List<dynamic>`

## 0.0.3+2

- Update documentation.

## 0.0.3

- [media_metadata_retriever](https://github.com/trungduc102/flutter_media_metadata) is now [flutter_media_metadata](https://github.com/trungduc102/media_metadata_retriever).
- Added Linux support with album arts.
- Uses [MediaInfoLib](https://github.com/MediaArea/MediaInfoLib) on Linux.

## 0.0.1+4

- Updated Metadata class structure.
- Now bitrate & duration in stored in Metadata itself.

## 0.0.1+3

- More minor changes.

## 0.0.1+2

- Minor updates to documentation.

## 0.0.1

- Support for retriving metadata of a media file in Android.
- Uses [MediaMetadataRetriever](https://developer.android.com/reference/android/media/MediaMetadataRetriever).
