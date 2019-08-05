
<!-- README.md is generated from README.Rmd. Please edit that file -->

# crap

<!-- badges: start -->

![](http://img.shields.io/badge/cool-useless-green.svg) [![Travis build
status](https://travis-ci.org/coolbutuseless/crap.svg?branch=master)](https://travis-ci.org/coolbutuseless/crap)
[![Codecov test
coverage](https://codecov.io/gh/coolbutuseless/crap/branch/master/graph/badge.svg)](https://codecov.io/gh/coolbutuseless/crap?branch=master)
<!-- badges: end -->

The goal of `crap` is to set up some tutorial stuff.

  - Make project public on github
  - `usethis::use_travis()` - this will
      - Add a badge to the README.Rmd
      - Pop open a window on `travis.org`
          - Flick the switch to active travis for this project
      - commit, push and wait for travis to complete a full build (just
        to be sure).
          - Badge on github should change from `Build:Unknown` to
            `Build:Passing`
  - `usethis::use_coverage()` **Must be done after TravisCI is added**
      - Need to add a snippet to `.travis.yml`

<!-- end list -->

    after_success:
        - Rscript -e 'covr::codecov()'
