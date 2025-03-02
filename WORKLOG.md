#### 支持Mathjax https://myblackboxrecorder.com/use-math-in-hexo/

Step
npm uninstall hexo-math --save
npm uninstall hexo-renderer-mathjax --save

Step
npm install hexo-filter-mathjax --save

对部分支持MathJax的主题来说，只需在主题配置文件将相关配置项开启即可使用MathJax。但对很多主题，需要自己配置。hexo-filter-mathjax可以帮我们解决这个问题。


渲染引擎

npm install hexo-renderer-kramed --save

escape: 
/^\\([\\`*{}\[\]()#$+\-.!_>])/
escape:
/^\\([`*\[\]()# +\-.!_>])/,

意味着把`\#, \*`等符号改写成字面的符号；

(env310) Blog$ npm list | grep math
├── hexo-filter-mathjax@0.9.0
├── hexo-math@5.0.0
(env310) Blog$ npm list | grep renderer
├── hexo-renderer-ejs@2.0.0
├── hexo-renderer-marked@7.0.0
├── hexo-renderer-stylus@3.0.1

\$会被解释成 $直接写出来；
但是\\不会被解释成？

#### 油猴脚本爬取知乎专栏文章并转换数学公式为latex格式

#### 文件丢失的情况无法正常编译

https://github.com/iissnan/hexo-theme-next/issues/1214

#### 有几种相对路径的写法？

要保证引用的url为：

问题1=用img1实现；

解决方案1=post_asset_folder:true+asset_image+hexo clean=可以为每个项目生成一个images目录；+可以把原始的url去掉

markdown+绝对路径=post_asset_folder+markdown语法中的路径名改成指定的目录

markdown+相对路径=post_asset_folder:false+images/reinforcement/images-1.png


问题1=blog路径不对+url_for
