# tutorial dependencies

|project|license [^_l]|description [dependencies]|version|source|diff [^_d]|
|-------|-------------|--------------------------|-------|------|----------|
|<a id='tutorial' />[tutorial](https://github.com/smanders/tutorial)|[MIT](https://github.com/externpro/tutorial?tab=MIT-1-ov-file#readme 'MIT License')|A simple externpro tutorial project [pvt deps: _fmt, spdlog, nlohmann_json_]| |[upstream](https://github.com/externpro/tutorial 'github.com/externpro/tutorial')|  [patch]|
|<a id='fmt' />[fmt](https://fmt.dev/)|[MIT](https://github.com/fmtlib/fmt?tab=MIT-1-ov-file#readme 'MIT License')|A modern formatting library|[xpv12.1.0.6](https://github.com/externpro/fmt/releases/tag/xpv12.1.0.6 'release')|[repo](https://github.com/externpro/fmt 'github.com/externpro/fmt') [upstream](https://github.com/fmtlib/fmt 'github.com/fmtlib/fmt')|[diff](https://github.com/externpro/fmt/compare/12.1.0...xpv12.1.0.6 'github.com/externpro/fmt/compare/12.1.0...xpv12.1.0.6') [patch]|
|<a id='spdlog' />[spdlog](https://github.com/gabime/spdlog/wiki)|[MIT](https://github.com/gabime/spdlog?tab=License-1-ov-file 'MIT License')|Fast C++ logging library [deps: _Threads, fmt_]|[xpv1.17.0.6](https://github.com/externpro/spdlog/releases/tag/xpv1.17.0.6 'release')|[repo](https://github.com/externpro/spdlog 'github.com/externpro/spdlog') [upstream](https://github.com/gabime/spdlog 'github.com/gabime/spdlog')|[diff](https://github.com/externpro/spdlog/compare/v1.17.0...xpv1.17.0.6 'github.com/externpro/spdlog/compare/v1.17.0...xpv1.17.0.6') [patch]|
|<a id='nlohmann_json' />[nlohmann_json](https://json.nlohmann.me)|[MIT](https://github.com/nlohmann/json/blob/develop/LICENSE.MIT 'MIT License')|JSON for Modern C++|[xpv3.12.0.4](https://github.com/externpro/nlohmann_json/releases/tag/xpv3.12.0.4 'release')|[repo](https://github.com/externpro/nlohmann_json 'github.com/externpro/nlohmann_json') [upstream](https://github.com/nlohmann/json 'github.com/nlohmann/json')|[diff](https://github.com/externpro/nlohmann_json/compare/v3.12.0...xpv3.12.0.4 'github.com/externpro/nlohmann_json/compare/v3.12.0...xpv3.12.0.4') [patch]|
|<a id='Threads' />[Threads](https://cmake.org/cmake/help/latest/module/FindThreads.html)|[LGPL-2.1-or-later](https://spdx.org/licenses/LGPL-2.1-or-later.html 'GNU Lesser General Public License v2.1 or later')|Finds and determines the thread library of the system for multithreading support|[xpv1.0.4](https://github.com/externpro/Threads/releases/tag/xpv1.0.4 'release')|[repo](https://github.com/externpro/Threads 'github.com/externpro/Threads')|[diff](https://github.com/externpro/Threads/compare/v0...xpv1.0.4 'github.com/externpro/Threads/compare/v0...xpv1.0.4') [bin]|

![deps](xprodeps.svg 'dependencies')

Dependency version check: all 5 parent-manifest versions match pinned versions.

|diff  |description|
|------|-----------|
|patch |diff modifies/patches existing cmake|
|intro |diff introduces cmake|
|auto  |diff adds cmake to replace autotools/configure/make|
|native|diff adds cmake but uses existing build system|
|bin   |diff adds cmake to repackage binaries built elsewhere|
|fetch |diff adds cmake and utilizes FetchContent|

[^_l]: see [SPDX License List](https://spdx.org/licenses/ '') for a list of commonly found licenses
[^_d]: see table above with description of diff
