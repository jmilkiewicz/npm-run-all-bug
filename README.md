# npm-run-all-bug



* `npm run-script test:t --npm-run-all-bug:reporter=nyan` 
 configuration variables are overwritten so one shall see test report in `nyan` format
* `npm test --npm-run-all-bug:reporter=nyan` and `npm run-script test-2 --npm-run-all-bug:reporter=nyan` 
 configuration variables are NOT overwritten so mocha output would be in `spec` format as specified in package.json config section
