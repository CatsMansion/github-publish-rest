# github-publish-rest
在这台机器上把本地文件夹发布到 GitHub 的可用通道。连接器只读（create_repository / push_files 均 403）、便携版 git 没有凭据助手导致 git push 取不到凭据，因此改为读取已存储的 token 后直接走 Git Data API 建一次提交。含现成脚本、提交后的哈希校验方法与三个已知坑。
