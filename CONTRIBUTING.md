# Contributing

The MapLibre TileJSON specification is an open specification maintained by MapLibre. You are welcome to contribute to this specification.

### Questions and Contributing

All specification development happens at https://github.com/maplibre/tilejson-spec. For general questions relating to the specification please feel free to create a new [issue](https://github.com/maplibre/tilejson-spec/issues).

### Proposing Changes

Every substantial change of the specification (things that are not just typo fixes) require a design proposal. Please open an Issue with a design propsal first.

- Editorial changes that clarify the specification are encouraged. Edits can be submitted as a pull request against the `main` branch of the latest version of the specification. Review and discussion of the proposed changes will take place on this pull request. Changes may warrant a bump in the `minor` version of the specification.

- Technical changes to the specification are an important part of the evolution of the standard. Technical changes imply new requirements for tools that create and/or read the format. Therefore a technical change requires the `major` version to be incremented and will be carefully reviewed and considered by implementors of the specification. Technical changes are best discussed in individual [issues](https://github.com/maplibre/tilejson-spec/issues) prior to a change in the specification. Please be concise in any suggestions and read existing issues prior to posting.

### Syntax Notes

Consideration should be taken over the uses of the keywords as described in [RFC 2119](https://www.ietf.org/rfc/rfc2119.txt). The use of these words must be capitalized to stress their meaning through out the specification.

### Releasing A New Version

The following is the suggested way to release a new version of the specification.

Upon determination that a significant need for a version change is required a pull request to the specification should be opened. The branch from which the pull request originates should be named clearly to note it is a request for a new version of the specification. For example a branch of `v3.0.0-development` would specify the grouping of changes for the `v3.0.0` specification. This pull request should create a new folder for the version of the specification that will be created, in this instance the folder would be named `3.0.0`. Within this folder should be the:
- `schema.json` file for the version
- `README.md` file that is a full update of the specification. Optionally include README translations - `README-{language code}.md`
- `example/` directory with JSON file examples

The pull request should provide a clear explanation of the intent for the new version of the specification. All associated issues should be linked in the pull request. Suggested changes to the branch of the development version will be accepted in the form of a pull request to that branch.
Once all issues with the pull request have been addressed the pull request may be merged into the master branch.

Update the `CHANGELOG.md` with the date of release of the official specification in a new commit to the `main` branch. Once this is done, create an official tag of the release on github.

```
    git tag -a v2.0.0 -m "v2.0.0"
    git push --tags
```

### Authors

If you make a change and wish to be added to the list of authors please add yourself to the README.md. (Note: It is alphabetical by last name).
