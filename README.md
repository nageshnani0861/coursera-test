# coursera-test
coursera repository
jekyll-theme-minimal

on: 
on:
  push:
  pull_request:
    types: [opened, synchronize]
@@ -8,9 +8,10 @@ jobs:
    name: script/cibuild
    steps:
      - uses: actions/checkout@v2
      - uses: actions/setup-ruby@v1
      - uses: ruby/setup-ruby@v1
        with:
          ruby-version: 2.7
          bundler-cache: true
      - name: build
        run: script/bootstrap
      - name: test
