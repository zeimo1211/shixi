```title
YQY的实习小帮手
```




# 使用说明

- 运行main.py来启动图形化界面启动后需要选择 ***学号-姓名*** 文件夹下的识别信息txt文件,如***Image_419_clustered.txt*** ,选择后会自动根据选择的txt文件读取识别信息,通过字典网站获取对应的满文图片,存储在***Image_419_result*** 文件夹下,该文件夹会在 ***学号-姓名*** 文件夹下被创建,等待获取图片完成后会进入图形化界面。

- 图形化界面的左侧图片为字典网站的检索结果，右侧图片为需要标注的图片，两张图片对应的编号一致。通过点击“正确”按钮或“错误”按钮来设置对错，当点击“下一个“按钮后，右侧需要标注的文件会根据 ***正确与否***、***页号***、***列号***、***行号***和***txt文件中对应编号的识别结果***来命名。

- 图形化界面中的列号输入框和行号输入框默认值都为1，当点击“下一个” 按钮后，行号自动加一，若需要环列，则点击”下一列“按钮，列号加1，行号被重设为1。

- 若已经有部分图片已被标注，使用步骤与上述步骤相同，启动后会从第一个没有被标注的图片开始进行标注，由于***不是从第一个图片开始，因此需要手动设置列号和行号***

# 注意事项

- 如果原始的图片编号和txt文件中的编号不一致，需要手动修改图片的编号使其与txt文件中的编号一致。
- 路径是根据默认的文件夹结构进行获取，若文件夹结构改变，会导致路径错误。
- 若出现 *获取出错：list index out of range* 提示，说明是网络问题，未能获取到图片。
- 标注完成后注意删除result文件夹。

