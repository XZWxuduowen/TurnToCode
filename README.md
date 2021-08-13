# TurnToCode


代码筛选工具 ,根据标签自动筛选出指定的支线代码         （负责人：许振文       开发状态：已经完成）
1)规则



 #if DEBUG // turn_to_code:202108101735

     【测试代码】

 #else // turn_to_code:202108101735

     【正式代码】

 #endif // turn_to_code:202108101735



测试代码的标签 ： #if DEBUG // turn_to_code:202108101735
正式代码的标签 ： #else // turn_to_code:202108101735
语句结束的标签 ： #endif // turn_to_code:202108101735

注意项：单行中的标签，后缀不允许添加任何内容，否则经过本工具筛选后，会保留单行中非标签的内容，从而导致代码运行报错





2)使用教程

教程在README上，比如相应的命令:

TurnToCode --help

TurnToCode -p xxxx -i xxxx -f xxxx -n xxxx -s xxxx



xuzhenwendeMacBook-Pro:~ xuzhenwen$ TurnToCode --help

[byxzw_debug] 当前运行环境为：Release

版本号为：1.0.0

usage: turnToCode [-h] -p PROJECT -i INDEX [-f FILTERPATHS] [-n FILTERNAME]

                  [-s FILTERSUFFIX]



*这是一个代码筛选工具 ,根据标签自动筛选出指定的支线代码*



optional arguments:

  -h, --help            show this help message and exit

  -p PROJECT, --project PROJECT

                        Enter project directory path

  -i INDEX, --index INDEX

                        Choose a code environment

  -f FILTERPATHS, --filterPaths FILTERPATHS

                        路径关键字过滤

  -n FILTERNAME, --filterName FILTERNAME

                        文件名关键字过滤

  -s FILTERSUFFIX, --filterSuffix FILTERSUFFIX

                        筛选指定文件格式



xuzhenwendeMacBook-Pro:~ xuzhenwen$ TurnToCode -p /Users/xuzhenwen/Documents/许多蚊/Job/aIT_lifeStyle/Python_XZW/03iOS自动化/xcode自动编译出包工具/TurnToCode/project -i 1

[byxzw_debug] 当前运行环境为：Release
版本号为：1.0.0

[byxzw_debug] turn_to_code path：/Users/xuzhenwen/Documents/许多蚊/Job/aIT_lifeStyle/Python_XZW/03iOS自动化/xcode自动编译出包工具/TurnToCode/project/AppDelegate.m

[byxzw_debug] TurnToCode successful!



技术支持与bug反馈的联系方式 ： QQ 450010152




