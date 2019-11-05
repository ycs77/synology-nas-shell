# Synology NAS 輔助腳本

新增 `~/bin` 資料夾來儲存腳本，並註冊到 PATH (`[user]` 替換成用戶名)：

```bash
vim ~/.bashrc

# 新增PATH
export PATH="$PATH:/var/services/homes/[user]/bin"
```

## phpon & phpoff

Synology 預設的 PHP cli 版本是 5，但平常使用的時候需要 PHP 7。

切換成 PHP cli 7

```bash
sudo phpon
```

切換回預設的 PHP cli 5

```bash
sudo phpoff
```
