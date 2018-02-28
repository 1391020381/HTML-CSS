# [PostCSS](https://github.com/postcss/postcss#usage)
1. 组织
2. 优化
3. 构建
4. 维护

# PostCSS<PostCSS 所能执行的任务非常多，同时涵盖了传统意义上的预处理和后处理。>
  1. 模块化
  2. 加前缀
  3. 兼容性
# PostCSS插件
  1. Autoprefixer<其作用是为 CSS 中的属性添加浏览器特定的前缀>
  2.  cssnext 
     * 允许开发人员在当前的项目中使用 CSS 将来版本中可能会加入的新特性。cssnext 负责把这些新特性转译成当前浏览器中可以使用的语法
     * cssnext 中已经包含了对 Autoprefixer 的使用，因此使用了 cssnext 就不再需要使用 Autoprefixer。
   3. cssnano <cssnano 会压缩你的 CSS 文件来确保在开发环境中下载量尽可能的小。> 
   4. PostCSS Sprites <将扫描你CSS中使用的所有图像，自动生成优化的 Sprites 图像和 CSS Sprites 代码>