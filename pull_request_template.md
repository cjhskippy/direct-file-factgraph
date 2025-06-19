## Description

### What changed

<-- Tell us what you changed in the PR -->

### Motivation and context

<-- Tell us why the change is important -->

## Tests

### Scala tests (if applicable)

- [ ] New tests were added to `direct-file-factgraph/direct-file/fact-graph-scala/shared/src/test/...` that cover this functionality
- [ ] `sbt test`, `sbt scalafmt`, `sbt compile`, `sbt clean`, and `sbt fastOptJS` all ran successfully.
- [ ] I have run `npm run copy-transpiled-js` from `/direct-file/df-client/df-client-app`
- [ ] I have run `docker-compose build` from `/direct-file/df-client/df-client-app`

### Fact dictionary tests (for all changes)

- [ ] I have added fact dictionary tests as appropriate.
- [ ] I have run `npm run generate-fact-dictionary` from `/direct-file-factgraph/direct-file/df-client/df-client-app`
- [ ] I have run `npm run test factDictionaryTests` from `/direct-file-factgraph/direct-file/df-client/df-client-app/src/test` and all tests pass.

### Manual tests

Describe how you verified that your changes worked as expected, if you did so outside of the automated tests. 

## Is there anything reviewers should look at carefully?

## Are there any loose ends or TODO items for the future?

