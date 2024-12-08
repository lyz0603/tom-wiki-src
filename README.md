# Tom Wiki

## 前言

鉴于古猿乱起外号，犯下的罪行令人发指，所以搞了个古猿百科记载~~他~~它的罪行。

## 贡献

### 准备

1. 一台电脑，装有[git](https://git-scm.com/book/zh/v2/%E8%B5%B7%E6%AD%A5-%E5%AE%89%E8%A3%85-Git)和[hugo](https://www.gohugo.org/)
2. 能用的大脑
3. pull/push/访问GitHub没问题的网络，若有问题可以使用[开发者边车](https://github.com/docmirror/dev-sidecar)~~（不过你怎么看到这篇文章的）~~
4. 没被古猿吃掉的手

### 操作

```bash
git clone https://github.com/lyz0603/tom-wiki-src.git --recursive
cd ./tom-wiki-src
hugo server -D
# 对 content 进行修改，观察 http://localhost:1313/ ，满意后 Ctrl+C 结束
cd ./pulic/
rm -rf !(.git/)
cd ..
hugo
git add -A
git commit -m "..."
cd ./pulic/
git add -A
git commit -m "..."
git push -u origin main
cd ..
git push -u origin main
```
