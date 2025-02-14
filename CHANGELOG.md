## [7.5.4](https://github.com/junrar/junrar/compare/v7.5.3...v7.5.4) (2022-11-04)


### Bug Fixes

* cannot extract large files (2G+) via InputStream ([cbbe99c](https://github.com/junrar/junrar/commit/cbbe99c45b6db8f2c2c8bec99db574729c0070c3)), closes [#104](https://github.com/junrar/junrar/issues/104)


### Performance Improvements

* improve copy string performance ([8e87641](https://github.com/junrar/junrar/commit/8e876416c5e6055eb7a9acce887f95a63e8c937b))

## [7.5.3](https://github.com/junrar/junrar/compare/v7.5.2...v7.5.3) (2022-08-08)


### Bug Fixes

* check validity of mark header and end archive header ([6c7dc7a](https://github.com/junrar/junrar/commit/6c7dc7af33e8a77b16ab2b12731be739994592e1))
* more checks on invalid headers ([cc33b6c](https://github.com/junrar/junrar/commit/cc33b6c179daa4a79899cec897857995bd6d1400))

## [7.5.2](https://github.com/junrar/junrar/compare/v7.5.1...v7.5.2) (2022-05-31)


### Bug Fixes

* cannot extract empty files to InputStream ([#90](https://github.com/junrar/junrar/issues/90)) ([c95a211](https://github.com/junrar/junrar/commit/c95a211a47466b2ca2f568edbb22dc976b22031d)), closes [#88](https://github.com/junrar/junrar/issues/88)

## [7.5.1](https://github.com/junrar/junrar/compare/v7.5.0...v7.5.1) (2022-04-28)


### Bug Fixes

* out of bounds read on corrupt extended time ([1d52d5d](https://github.com/junrar/junrar/commit/1d52d5d308afa607bce6fc5253bf950193e35852)), closes [#86](https://github.com/junrar/junrar/issues/86)

# [7.5.0](https://github.com/junrar/junrar/compare/v7.4.1...v7.5.0) (2022-03-20)


### Bug Fixes

* crc errors on audio data decompression ([15f4afa](https://github.com/junrar/junrar/commit/15f4afa23eff69c2e0f3c906815777abf5ac267c))
* NPE on audio data decompression ([952436b](https://github.com/junrar/junrar/commit/952436b204614a747fe8a401d213196cd326d818))


### Features

* parse extended time ([d5cc784](https://github.com/junrar/junrar/commit/d5cc784c937f461be1e71a7a92b4018af8aef8c7))
* use thread pool for getInputStream ([a3383b0](https://github.com/junrar/junrar/commit/a3383b0dc4db5c5c29334abadd42688fa5ea583b))


### Performance Improvements

* performance optimizations ([36a5883](https://github.com/junrar/junrar/commit/36a58836c3abd042a9c2cb544d7bbf8aec7beeb7))
* reduce array creation, unsigned shifts ([d276f93](https://github.com/junrar/junrar/commit/d276f937c0c328a4450164d138b3bc60db4f2542))

## [7.4.1](https://github.com/junrar/junrar/compare/v7.4.0...v7.4.1) (2022-01-27)


### Bug Fixes

* invalid subheader type would throw npe and make the extract loop ([7b16b3d](https://github.com/junrar/junrar/commit/7b16b3d90b91445fd6af0adfed22c07413d4fab7)), closes [#73](https://github.com/junrar/junrar/issues/73)

## [7.4.1](https://github.com/junrar/junrar/compare/v7.4.0...v7.4.1) (2022-01-27)


### Bug Fixes

* invalid subheader type would throw npe and make the extract loop ([7b16b3d](https://github.com/junrar/junrar/commit/7b16b3d90b91445fd6af0adfed22c07413d4fab7)), closes [#73](https://github.com/junrar/junrar/issues/73)

# [7.4.0](https://github.com/junrar/junrar/compare/v7.3.0...v7.4.0) (2020-11-01)


### Features

* make getContentsDescription usable with a Stream ([7a221f7](https://github.com/junrar/junrar/commit/7a221f7686e79d6d5fbd5fbc7573796b4057119d)), closes [#56](https://github.com/junrar/junrar/issues/56)

# [7.3.0](https://github.com/junrar/junrar/compare/v7.2.0...v7.3.0) (2020-08-03)


### Features

* support header-encrypted archive ([c2a24f3](https://github.com/junrar/junrar/commit/c2a24f3c509c4a10b8a03377e117a50013fdb16b))

# [7.2.0](https://github.com/junrar/junrar/compare/v7.1.0...v7.2.0) (2020-07-28)


### Features

* add FileHeader.getFileName ([b6da583](https://github.com/junrar/junrar/commit/b6da583ffbb861219fe20877fb78bf5092996914)), closes [#34](https://github.com/junrar/junrar/issues/34) [#53](https://github.com/junrar/junrar/issues/53)

# [7.1.0](https://github.com/junrar/junrar/compare/v7.0.0...v7.1.0) (2020-07-27)


### Features

* multi-part extraction from inputstream ([9ee32ea](https://github.com/junrar/junrar/commit/9ee32eafc12436b625c020ac96cd2a4e091af972)), closes [#52](https://github.com/junrar/junrar/issues/52)

# [7.0.0](https://github.com/junrar/junrar/compare/v6.0.1...v7.0.0) (2020-07-25)


### Code Refactoring

* cleanup public entry points ([70499bb](https://github.com/junrar/junrar/commit/70499bb89442098048af183ab3ca77fca0fd92da))
* move Volume classes to volume package ([c2405e0](https://github.com/junrar/junrar/commit/c2405e04e1dbeb06b01dff419189105321d243e5))
* simplify IO ([b59fc78](https://github.com/junrar/junrar/commit/b59fc78f10f9b650d73ad72a60e139adb4dff09e))


### Features

* add password parameter for inputstream archives ([b218bb9](https://github.com/junrar/junrar/commit/b218bb973ae2ddbb59cae7ba7558b7accab70091))
* check if archive is password protected ([c1b7728](https://github.com/junrar/junrar/commit/c1b77289ccfcf36061513ae419cf1770b76c0d57))
* support for password protected archives ([4402afc](https://github.com/junrar/junrar/commit/4402afc0c5a6a53e8dc10956b902f2fe0e960c7e)), closes [#48](https://github.com/junrar/junrar/issues/48) [#40](https://github.com/junrar/junrar/issues/40)


### BREAKING CHANGES

* public API changed
* public API changed
* name of classes have changed

## [6.0.1](https://github.com/junrar/junrar/compare/v6.0.0...v6.0.1) (2020-07-21)


### Bug Fixes

* inaccurate file times ([b1f9638](https://github.com/junrar/junrar/commit/b1f96385ff1738c1488b26968f71413f2a5085d4)), closes [edmund-wagner/junrar#20](https://github.com/edmund-wagner/junrar/issues/20)

# [6.0.0](https://github.com/junrar/junrar/compare/v5.0.0...v6.0.0) (2020-07-19)


### Code Refactoring

* exception inheritance ([aece14d](https://github.com/junrar/junrar/commit/aece14d42ec402e40f6600cbdb576b717a4220bc))
* migrate from commons-logging to SLF4J ([e6f461b](https://github.com/junrar/junrar/commit/e6f461b60875e582ac54ee4b8b3a23744d5d97c0))
* remove deprecated code ([99d4399](https://github.com/junrar/junrar/commit/99d43991023ca8d510663f9816a88c7796f7b210))


### Reverts

* rollback dependency-analysis plugin version ([29f8ab5](https://github.com/junrar/junrar/commit/29f8ab5ac250666823324e7b3ded5f1461b8290d))


### BREAKING CHANGES

* migrate from commons-logging to SLF4J
* RarException has changed
* remove ExtractArchive classes, use Junrar.extract instead

# [5.0.0](https://github.com/junrar/junrar/compare/v4.0.0...v5.0.0) (2020-07-18)


### Bug Fixes

* nullPointerException on corrupt headers ([b721589](https://github.com/junrar/junrar/commit/b721589640bdbf142b5e2daebe5fc0d5c8fab388)), closes [#36](https://github.com/junrar/junrar/issues/36) [#45](https://github.com/junrar/junrar/issues/45)


### Build System

* use gradle instead of maven ([9aa5794](https://github.com/junrar/junrar/commit/9aa579434ed50ee4150c696ba359ac7fa3cb557f)), closes [#20](https://github.com/junrar/junrar/issues/20)


### Code Refactoring

* remove VFS support ([3bbe8ed](https://github.com/junrar/junrar/commit/3bbe8eda39fb7d289bfacfda97169de035112416)), closes [#41](https://github.com/junrar/junrar/issues/41)


### BREAKING CHANGES

* carved-out into its own repo
* minimum java version bumped from 6 to 8
