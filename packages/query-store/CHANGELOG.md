# @evidence-dev/query-store

## 2.0.0-usql.22

### Patch Changes

- Updated dependencies [15248699]
  - @evidence-dev/universal-sql@2.0.0-usql.24

## 2.0.0-usql.21

### Patch Changes

- Updated dependencies [9603c4e7]
  - @evidence-dev/universal-sql@2.0.0-usql.23

## 2.0.0-usql.20

### Patch Changes

- Build before publishing this time

## 2.0.0-usql.19

### Patch Changes

- e2162851: Clean up logs

## 2.0.0-usql.18

### Patch Changes

- 391282e5: QueryStore now uses a factory pattern to enforce caching

## 2.0.0-usql.17

### Patch Changes

- Force version bump

## 2.0.0-usql.16

### Patch Changes

- 16a17086: Fix issue with initial data

## 2.0.0-usql.15

### Patch Changes

- 4c6eae53: Minor updates to intitaldata behavior
- ba0d6f50: When fetching data for the 2nd time, the result promise from the first instance is returned, instead of undefined
- Updated dependencies [9132146b]
  - @evidence-dev/universal-sql@2.0.0-usql.22

## 2.0.0-usql.14

### Patch Changes

- 7a5225be: QueryStore more aggresively loads metadata; and ignore 0-length initial data

## 2.0.0-usql.13

### Patch Changes

- 583cea9e: Properly retrieve column types from QueryStores

## 2.0.0-usql.12

### Patch Changes

- Updated dependencies [2aaef5fb]
  - @evidence-dev/universal-sql@2.0.0-usql.21

## 2.0.0-usql.11

### Patch Changes

- Updated dependencies [cb74406a]
- Updated dependencies [d1ab5e62]
  - @evidence-dev/universal-sql@2.0.0-usql.20

## 2.0.0-usql.10

### Patch Changes

- Update package.json to use new datasource field
- Updated dependencies
  - @evidence-dev/universal-sql@2.0.0-usql.19

## 2.0.0-usql.9

### Patch Changes

- Updated dependencies [377abb4a]
  - @evidence-dev/universal-sql@2.0.0-usql.18

## 2.0.0-usql.8

### Patch Changes

- 840d1195: allow initialdata to saturate columns
- 6064fbbf: Loaded now means meta, length, and data, not just data
- Updated dependencies [840d1195]
- Updated dependencies [26ad2d2c]
  - @evidence-dev/universal-sql@2.0.0-usql.17

## 2.0.0-usql.7

### Patch Changes

- Updated dependencies [4d5735a2]
  - @evidence-dev/universal-sql@2.0.0-usql.16

## 2.0.0-usql.6

### Patch Changes

- Updated dependencies [b25a95d7]
  - @evidence-dev/universal-sql@2.0.0-usql.15

## 2.0.0-usql.5

### Patch Changes

- 6eb93816: QueryViewer now respects QueryStore loading staet
  QueryViewer now updates when query text hmr updates

  QueryStore now accepts initialError when SSR query fails

  SSR / QueryStore now swallow errors unless build:strict is enabled
  (e.g. the error propogates to the UI where the user can more easily find it in dev mode / regular builds)

- Updated dependencies [fd74bd3c]
  - @evidence-dev/universal-sql@2.0.0-usql.14

## 2.0.0-usql.4

### Patch Changes

- Updated dependencies [b5592a3f]
  - @evidence-dev/universal-sql@2.0.0-usql.13

## 2.0.0-usql.3

### Patch Changes

- Updated dependencies [0ba78b67]
- Updated dependencies [cd57ba69]
  - @evidence-dev/universal-sql@2.0.0-usql.12

## 2.0.0-usql.2

### Patch Changes

- 9bd1cd29: remove old workaround with a merged fix
- 130950d7: add client/build time guardrails
- Updated dependencies [130950d7]
- Updated dependencies [52d81ce2]
  - @evidence-dev/universal-sql@2.0.0-usql.11

## 2.0.0-usql.1

### Patch Changes

- 64d1405b: Loading state is now respected by Value and BigValue

## 2.0.0-usql.0

### Major Changes

- e1facffd: Add QueryStore concept

  - Loads data as it is requested, rather than all at page-load / build
  - Uses duckdb to get data length / column data
  - Ties metadata, mutation queries, and data together to make component development easier
  - Provides information regarding loading (and query errors in the future)

### Patch Changes

- 078fca3b: Error handling via QueryStores is more effective now
