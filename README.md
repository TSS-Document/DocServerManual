# 文档服务器手册
该服务器主要功能是,当指定gitbook仓库收到提交时,自动将其部署到web服务器中.

本文档github地址为https://github.com/TSS-Document/DocServerManual

## 环境
1. git
2. npm
2. gitbook
3. 你喜欢的`markdown`编辑器.推荐`atom`或`gitbook editor`

## 步骤
1. 在TssRequirement的organization中创建仓库,url为https://github.com/TSS-Document
2. 本地clone仓库,在 `.git`同级目录执行`gitbook init`
4. 创建.gitignore文件,写入内容
   ```
   /_book
   ```

   
3. 创建`styles`文件夹,在其中添加`website.css`文件,内容为

  ```css
    .book .book-summary, .book .book-body,code{
      font-family:"Microsoft YaHei UI",
                  "Microsoft Yahei",
                  "PingFang SC",
                  "Lantinghei SC",
                  "Hiragino Sans GB",
                  "WenQuanYi Micro Hei",
                  "WenQuanYi Zen Hei",
                  "Noto Sans CJK SC",
                  "Microsoft JhengHei UI",
                  "Microsoft JhengHei",
                  "PingFang TC",
                  "Lantinghei TC",
                  "Noto Sans CJK TC",
                  "Helvetica Neue",
                  Helvetica,
                  Arial,
                  sans-serif;
    }
  ```

  >可选,这样做是为了让字体变好看
3. commit and push
4. 约20秒后,http://115.29.184.56:10000/html 中可查看到编译好的网页
