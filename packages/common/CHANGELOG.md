# Change Log

All notable changes to this project will be documented in this file.
See [Conventional Commits](https://conventionalcommits.org) for commit guidelines.

## [0.7.3](https://github.com/Sphereon-Opensource/OID4VCI/compare/v0.7.2...v0.7.3) (2023-09-30)

**Note:** Version bump only for package @sphereon/oid4vci-common





## [0.7.2](https://github.com/Sphereon-Opensource/OID4VCI/compare/v0.7.1...v0.7.2) (2023-09-28)


### Bug Fixes

* id lookup against server metadata not working ([592ec4b](https://github.com/Sphereon-Opensource/OID4VCI/commit/592ec4b837898eb3022d19479d79b6065e7a0d9e))





## [0.7.1](https://github.com/Sphereon-Opensource/OID4VCI/compare/v0.7.0...v0.7.1) (2023-09-28)


### Bug Fixes

* Better match credential offer types and formats onto issuer metadata ([4044c21](https://github.com/Sphereon-Opensource/OID4VCI/commit/4044c2175b4cbee16f44c8bb5499bba249ca4993))
* Fix credential offer matching against metadata ([3c23bab](https://github.com/Sphereon-Opensource/OID4VCI/commit/3c23bab83569e04a4b5846fed83ce00d68e8ddce))
* Fix credential offer matching against metadata ([b79027f](https://github.com/Sphereon-Opensource/OID4VCI/commit/b79027fe601ecccb1373ba399419e14f5ec2d7ff))
* relax auth_endpoint handling. Doesn't have to be available when doing pre-auth flow. Client handles errors anyway in case of auth/par flow ([cb5f9c1](https://github.com/Sphereon-Opensource/OID4VCI/commit/cb5f9c1c12285508c6d403814d032e8883a59e7d))





# [0.7.0](https://github.com/Sphereon-Opensource/OID4VCI/compare/v0.6.0...v0.7.0) (2023-08-19)

### Bug Fixes

- fix credential request properties ([0037025](https://github.com/Sphereon-Opensource/OID4VCI/commit/0037025ef27d3a1fa7c68954b1f87e660ef0c82c))
- Revise well-known metadata retrieval for OID4VCI, OAuth 2.0 and OIDC. fixes [#62](https://github.com/Sphereon-Opensource/OID4VCI/issues/62) ([a750cc7](https://github.com/Sphereon-Opensource/OID4VCI/commit/a750cc76e084f12aeb58f2b1ac44b1bb5e69b5ae))

### Features

- Integrate ssi-express-support to allow for future authn/authz. Also moved endpoints to functions, so solutions can include their own set of endpoints ([c749aba](https://github.com/Sphereon-Opensource/OID4VCI/commit/c749ababd4bec567d6aeeda49b76f195ec792201))

# [0.6.0](https://github.com/Sphereon-Opensource/OID4VCI/compare/v0.4.0...v0.6.0) (2023-06-24)

### Bug Fixes

- added a couple of todos for handling v11, plus changed the getIssuer method to throw exception if nothing is found, and some other pr notes ([091786e](https://github.com/Sphereon-Opensource/OID4VCI/commit/091786e31246da16f6c9385fc13e7fd3e01664dc))
- added disable eslint comments in three places ([0e3ffdb](https://github.com/Sphereon-Opensource/OID4VCI/commit/0e3ffdb3a434e142d3bd8d0e04ca0b2b0f8f73e3))
- made v1_0.09 types strict and added a few utility methods to it for ease of access ([9391f31](https://github.com/Sphereon-Opensource/OID4VCI/commit/9391f317ee41068b823901036c3ac7d4b33ce6dd))
- Many v11 fixes on server and client side ([08be1ed](https://github.com/Sphereon-Opensource/OID4VCI/commit/08be1ed009fb80e910cffa2e4cf376758798b27e))
- PAR objects where in the wrong locations and one had a wrong name ([24f98e7](https://github.com/Sphereon-Opensource/OID4VCI/commit/24f98e75137cf70595753cbcf77159584d7ebe08))
- prettier, plus some type casting in test/mock files for v9 ([162af38](https://github.com/Sphereon-Opensource/OID4VCI/commit/162af3828b3dc826dc3cd5adffe3dab61925ad33))
- removed type support for mso_mdoc ([867073c](https://github.com/Sphereon-Opensource/OID4VCI/commit/867073ccf3612e6ad869dbc662c791b292fe06ca))
- rename jwt_vc_json_ld to jwt_vc_json-ld ([a366bef](https://github.com/Sphereon-Opensource/OID4VCI/commit/a366bef5a7bda052de6ffa201186e02b70447a79))

### Features

- Add status support to sessions ([02c7eaf](https://github.com/Sphereon-Opensource/OID4VCI/commit/02c7eaf69af441e15c6302a9c0f2874d54066b32))
- Add support for alg, kid, did, did document to Jwt Verification callback so we can ensure to set proper values in the resulting VC. ([62dd947](https://github.com/Sphereon-Opensource/OID4VCI/commit/62dd947d0e09360719e6f704db33d766dff2363a))
- Add support for background_image for credentials ([a3c2561](https://github.com/Sphereon-Opensource/OID4VCI/commit/a3c2561c7596ad7303467528d92cdaa033c7af94))
- Add supported flow type detection ([100f9e6](https://github.com/Sphereon-Opensource/OID4VCI/commit/100f9e6ccd7c53353f2876be81df4d6e3f7efde4))
- Add VCI Issuer ([5cab075](https://github.com/Sphereon-Opensource/OID4VCI/commit/5cab07534e7a8b340f7a05343f56fbf091d64738))
- added better support (and distinction) for types v1.0.09 and v1.0.11 ([f311258](https://github.com/Sphereon-Opensource/OID4VCI/commit/f31125865a3d63ce7719f790fc5ac74fea7f9ade))
- added callback function for issuing credentials ([c478788](https://github.com/Sphereon-Opensource/OID4VCI/commit/c478788d3d3d2414073eedddd9d43cc3d593ee1b))
- added error code invalid_scope ([e7864d9](https://github.com/Sphereon-Opensource/OID4VCI/commit/e7864d96476ae8ff21867646c0943975b773d7d5))
- Added new mock data from actual issuers, fixed a small bug with v1_0_08 types, updated v1_0_08 types to support data from jff issuers ([a6b1eea](https://github.com/Sphereon-Opensource/OID4VCI/commit/a6b1eeaabc0f34cc13a79cf967a8c35a6d8dc7f5))
- Added new tests for CredentialRequestClient plus fixed a problem with CredentialOfferUtil. a CredentialRequest can have no issuer field ([50f2292](https://github.com/Sphereon-Opensource/OID4VCI/commit/50f22928426761cc3bf5d973d1f15fea407a9175))
- added support for creating offer deeplink from object and test it. plus some refactors ([a87dcb1](https://github.com/Sphereon-Opensource/OID4VCI/commit/a87dcb1ec10ea26a221d61ec0ffd4b4e098a594f))
- added support for v8 in our types (partially) to make old logics work ([4b5abf1](https://github.com/Sphereon-Opensource/OID4VCI/commit/4b5abf16507bcde0d696ea3948f816d9a2de13c4))
- added utility method for recognizing v1.0.11 objects ([ed6436e](https://github.com/Sphereon-Opensource/OID4VCI/commit/ed6436e3bd22307fe9f7b4411ff3c8086ddb940c))
- added VcIssuer and builders related to that ([c2592a8](https://github.com/Sphereon-Opensource/OID4VCI/commit/c2592a8846061c5791050a76e522f50e21f617de))
- Ass support to provide credential input data to the issuer whilst creating the offer to be used with a credential data supplier ([03d3e46](https://github.com/Sphereon-Opensource/OID4VCI/commit/03d3e46ab44b2e924320b6aed213c88d2ad161db))
- Issuer credential offer and more fixes/features ([0bbe17c](https://github.com/Sphereon-Opensource/OID4VCI/commit/0bbe17c13de4df95e2fd79b3470a746cc7a5374a))
- Support data supplier callback ([1c49cc8](https://github.com/Sphereon-Opensource/OID4VCI/commit/1c49cc80cfd83115956c7e9a040e12e814724e72))
- Translate v8 credentials_supported to v11 ([b06fa22](https://github.com/Sphereon-Opensource/OID4VCI/commit/b06fa221bed33e69aa76ae0234779f80314f2887))
