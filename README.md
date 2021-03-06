# Sinister Chicken Syndicate

[![Travis](https://img.shields.io/travis/lewismoten/sinister-chicken-syndicate.svg?style=flat-square&label=linux%20%26%20osx%20build)](https://travis-ci.org/lewismoten/sinister-chicken-syndicate)
[![AppVeyor](https://img.shields.io/appveyor/ci/lewismoten/sinister-chicken-syndicate/master.svg?style=flat-square&label=windows%20build)](https://ci.appveyor.com/project/lewismoten/sinister-chicken-syndicate)
[![Code Climate](https://codeclimate.com/github/lewismoten/Sinister-Chicken-Syndicate/badges/gpa.svg)](https://codeclimate.com/github/lewismoten/Sinister-Chicken-Syndicate)
[![Test Coverage](https://codeclimate.com/github/lewismoten/Sinister-Chicken-Syndicate/badges/coverage.svg)](https://codeclimate.com/github/lewismoten/Sinister-Chicken-Syndicate/coverage)
[![David](https://img.shields.io/david/lewismoten/sinister-chicken-syndicate.svg?style=flat-square)](https://david-dm.org/lewismoten/sinister-chicken-syndicate)
[![license](https://img.shields.io/badge/license-ISC-brightgreen.svg?style=flat-square)](https://raw.githubusercontent.com/lewismoten/sinister-chicken-syndicate/master/LICENSE.md)
[![Join the chat at https://gitter.im/lewismoten/sinister-chicken-syndicate](https://badges.gitter.im/lewismoten/sinister-chicken-syndicate.svg)](https://gitter.im/lewismoten/sinister-chicken-syndicate?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

A sample Node.js project with continuous integration support

# Setting up a new project

There are tests setup regarding the repository location and license. One you make a change to reflect the forked repository location or license, you will need to update all affected areas to get the tests to pass. See the `spec/project` folder for these tests.

This project is setup to integrate with services that you will need to configure with a forked repository:

1. Travis
 - Create an account, link your GitHub account, and import your repo.
 - Once a job is setup, go to the settings and add `CODECLIMATE_REPO_TOKEN` as an environment variable, and mark it so it is not displayed in the build log.
 - Travis Settings: `https://travis-ci.org/{user}/{repo}/settings`
 - Code Climate token: `https://codeclimate.com/repos/{repo id}/coverage_setup`. *Look at any language setup instructions to see the token.*
 - To skip a build, use `[ci skip]` in a commit
1. AppVeyor
- Create an account, link your GitHub account, and import your repo.
- To skip a build, use `[ci skip]` in a commit
1. Code Climate
- Create an account, link to github, and import your repo.
- Travis is used to report code coverage statistics to Code Climate.
- Code Climate uses and older version of eslint that is not compatible with some of the new rules. ESLint been disabled in `.codeclimate.yml`
1. David.
- No setup required.
1. Gitter
- Create an account, link your GitHub account, and import your repo.

# License

> Copyright (c) 2016, Lewis Edward Moten III
>
> Permission to use, copy, modify, and/or distribute this software for any purpose with or without fee is hereby granted, provided that the above copyright notice and this permission notice appear in all copies.
>
> THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
