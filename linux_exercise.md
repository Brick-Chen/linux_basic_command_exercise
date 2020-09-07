# Linux Exercise

### 假设在初始条件下位于用户目录(~)下。

#### 1.创建一个名称为cli-practice的目录

```
mkdir cli-practice
```

#### 2.在~/cli-practice下创建一个空白文件readme.md

```
cd ~/cli-practice
touch readme.md
```

#### 3.在~/cli-practice/readme.md中添加一行文本: Hi there, this is a readme file.
```
cd ~/cli-practice
echo "Hi there,this is a readme file.">> readme.md
```

#### 4.在 ~/cli-practice/readme.md 中追加一行文本：This is the second line of the readme file.  此时readme.md文件中包含两行文本。
```
cd ~/cli-practice
echo  "This is the second line of the readme file.">> readme.md
cat readme.md
```

#### 5.将 ~/cli-practice/readme.md 改名为readme.txt

```
mv ~/cli-practice/readme.md readme.txt
```

#### 6.创建目录 ~/cli-practice/document
```
mkdir ~/cli-practice/document
```

#### 7.将 ~/cli-practice/readme.txt 文件移动到 ~/cli-practice/document 中，并改名为 introduction.txt
```
mv ~/cli-practice/readme.txt ~/cli-practice/document/introduction.txt
```

#### 8.将 ~/cli-practice/document 中的 introduction.txt 文件在 ~/cli-practice/document 目录复制一份，并命名为 readme.txt
```
cp ~/cli-practice/document/introduction.txt ~/cli-practice/document/readme.txt
```

#### 9.使用 The quick brown fox jumps over a lazy dog 这行文本覆盖 ~/cli-practice/document/readme.txt 文件的内容。
```
cat ~/cli-practice/document/readme.txt
echo "The quick brown fox jumps over a lazy dog"> ~/cli-practice/document/readme.txt
cat ~/cli-practice/document/readme.txt
```

#### 10.将 ~/cli-practice/document 目录复制到 ~/cli-practice/docs，目录中的文件也要进行复制。
```
cp -r ~/cli-practice/document ~/cli-practice/docs
```

#### 11.删除 ~/cli-practice/document 目录及其中文件。
```
rm -rf ~/cli-practice/document
```

#### 12.创建 ~/cli-practice/parent/child/docs 目录。
```
mkdir -p ~/cli-practice/parent/child/docs
```

#### 13.将 ~/cli-practice/docs/introduction.txt 文件复制到~/cli-practice/parent/child/docs目录下
```
cp  ~/cli-practice/docs/introduction.txt ~/cli-practice/parent/child/docs
```
