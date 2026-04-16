# literature-clock
Clock using time quotes from the literature, based on work and idea by
        [Jaap Meijers](http://www.eerlijkemedia.nl/) ([E-reader clock](https://www.instructables.com/id/Literary-Clock-Made-From-E-reader/)).

Force light or dark theme with the `theme` query parameter. E.g. https://literature-clock.jenevoldsen.com?theme=dark

The working site is in the docs/ folder, and can be visited at http://literature-clock.jenevoldsen.com/. To run it locally you may need to serve docs/ with an HTTP server (e.g. `python3 -m http.server`) ... or just open index.html in Firefox (thanks [@gbear605](https://github.com/gbear605)).

> ℹ️ NB: Some quotes are potentially NSFW. See issue [#11](https://github.com/JohannesNE/literature-clock/issues/11).
> To filter out (most) NSFW quotes, use the `sfw` query parameter. E.g. https://literature-clock.jenevoldsen.com?sfw=true
> 

# Convert .csv quotes to .json quotes

Quotes are kept in `litclock_annotated.csv`. These are converted into a `.json` file for each minute with `csv_to_json.R`. To run the R script, install R and use the package manager, {packrat}, to install the correct version of the packages: `packrat::restore()`.

## Other related projects

- **[litime](https://github.com/ikornaselur/litime)** - A command line tool that shows a timely quote when it is executed.

# 文学时钟

基于 Jaap Meijers 的作品和创意开发的文学时间引用时钟
（[Jaap Meijers](http://www.eerlijkemedia.nl/)  的 [电子阅读器时钟](https://www.instructables.com/id/Literary-Clock-Made-From-E-reader/)）。

可通过 theme 查询参数强制切换亮色或暗色主题。例如：https://literature-clock.jenevoldsen.com?theme=dark

工作站点位于 docs/ 文件夹，可通过 http://literature-clock.jenevoldsen.com/ 访问。若要在本地运行，可能需要通过 HTTP 服务器（如 python3 -m http.server）来提供 docs/ 目录服务……或直接在 Firefox 中打开 index.html（感谢 @gbear605）。

> ℹ️ 注意：部分引用内容可能不适合在工作环境中查看（NSFW）。详见 Issue #11。
> 若需过滤（大部分）NSFW 引用，请使用 sfw 查询参数。例如：https://literature-clock.jenevoldsen.com?sfw=true
> 

# 将 .csv 引用转换为 .json 引用

引用内容存储在 litclock_annotated.csv 文件中。通过 csv_to_json.R 脚本可将其转换为每分钟对应的 .json 文件。运行该 R 脚本前，请先安装 R，并使用包管理器 {packrat} 安装指定版本的依赖包：packrat::restore()。
# 其他相关项目

- **[litime](https://github.com/ikornaselur/litime)** - 一款命令行工具，执行时会显示与当前时间匹配的引用。
