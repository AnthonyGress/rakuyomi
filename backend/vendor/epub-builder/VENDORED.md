# Vendored epub-builder

Source: epub-builder 0.8.3 from crates.io (https://crates.io/crates/epub-builder),
MPL-2.0 licensed (see LICENSE).

Local patch: adds `EpubBuilder::set_zip_comment` plus `Zip::set_comment`
(implemented for `ZipLibrary`), used by `shared/src/chapter_downloader.rs`
to tag generated EPUBs with the chapter id.

This replaces the former git dependency on
https://github.com/tachibana-shin/epub-builder, which no longer exists and
broke every CI build ("failed to authenticate when downloading repository").
