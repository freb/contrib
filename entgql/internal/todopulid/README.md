# todo example with PULIDs (Prefixed ULIDs).

`PULID`s are an identifier encoding scheme that builds upon the excellent ULID (Universally
Unique Lexicographically Sortable Identifier) scheme. ULIDs are base32 encoded and it may make sense in some cases to constrain the characters used for encoding the entity type prefix to the [same alphabet](https://github.com/oklog/ulid/blob/v2.0.2/ulid.go#L277) used for the ULID. If constrained to 2 characters for encoding the entity type, the number of types of entities that can be referenced with this scheme is `2^32` (1024).
