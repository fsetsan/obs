# i3wm でウィンドウサイズを調整したプロファイルを保存・復元する方法

i3wm ではウィンドウのレイアウトを保存し、後で復元することができます。以下の方法を試してみてください。

---

## 1. `i3-resurrect` を使う (推奨)
[i3-resurrect](https://github.com/JonnyHaystack/i3-resurrect) は、現在のウィンドウのレイアウトを保存・復元できるツールです。



### **インストール**
```sh
yay -S i3-resurrect
```
または手動で `~/.config/i3/scripts/` などにダウンロードしてもOK。

### **使い方**
#### **保存**
```sh
i3-resurrect save -w
```
またはワークスペースごとに保存:
```sh
i3-resurrect save -w 2
```

#### **復元**
```sh
i3-resurrect restore -w
```
またはワークスペース指定:
```sh
i3-resurrect restore -w 2
```

これでウィンドウのレイアウトが保存・復元できます。

---

