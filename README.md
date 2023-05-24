# Release Modpack docker action

This action releases a new version of a given modpack using the latest tagged version of the repository.

## Requirements
- Modpack must be hosted on Modrinth
- Releases must be provided in the format of `.mrpack` files, stored in a `releases` folder

## Inputs

## `modpack-id`

**Required** The ID of your modpack on Modrinth.

## `github-token`

**Required** An active OAuth token for Github. This should be provided as a secret.

## Outputs

## `success`

Whether the step succeeded

## `url`

The URL of the new modpack version

## Example usage

uses: clovercraft/release-modpack@v1
with:
  modpack-id: '#####'
  github-token: '######'