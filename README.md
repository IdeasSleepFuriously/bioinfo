# Bioinformatic_HW_1
## Notes
### What to learn
1. Programming Skill
2. NGS Data Analysis
3. Machine Learning
### How to learn
- In-class Learning ( 1.5h each week)
- Students: practice, experience sharing (Peer Learning) 
- After-class Study (3-5 hrs each week, ~50-80 hr)
### Introduction to the lesson
- Gene: segment of DNA?  In bioinfomatic we may say it is a segment of infomation.
- Genome: size vary form Mbp to Gbp.
- Big genome, few gene
	- why?   ncRNA(non-coding) such as miRNA
- Method: Sequencing 
	- History
	- NGS Sequencing
	- Output: Big and High-dimensional data
### \*Algorithm and Model
- Algorithm is a math way to create a model. There can be many different algorithms to achieve one goal, so we can choose the most effecient and convenient one to get desired result.
- Model is the output of an algorithm when combined with the data. It is used for prediction and in some extent is what we really want.
### Basic setup
#### load image: 
`docker load -i img_path`
#### create a container
`'docker run --name=bioinfo_tsinghua -dt -h bioinfo_docker --restart unless-'stopped -v host_path:/home/test/share xfliu1995/bioinfo_tsinghua:2`

- `docker run`： 用于启动一个新的容器。
- `--name=bioinfo_tsinghua`： 为容器指定一个名称，这里是 "bioinfo_tsinghua"。
- `-dt`： 这是两个选项的组合。 `-d` 表示在后台运行容器（detached mode），而 `-t` 表示为容器分配一个伪终端（pseudo-tty）。
- `-h bioinfo_docker`： 设置容器的主机名为 "bioinfo_docker"。
- `--restart unless-stopped`： 定义容器的重启策略。这里指定了容器除非手动停止，否则将在启动后自动重启。
- `-v host_path:/home/test/share`： 这是一个绑定挂载的选项，将主机上的路径 host_path 映射到容器内的路径 `/home/test/share`。这使得主机和容器之间可以共享文件。
- `xfliu1995/bioinfo_tsinghua:2`： 指定要运行的 Docker 镜像的名称及版本。这里是镜像 "xfliu1995/bioinfo_tsinghua" 的版本 "2"。
#### Run and exit the container
* run: `docker exec -it name bash`
* exit: exit
#### Maintain a container
* 检查 Docker 是否正常安装：`docker info`
* 查看当前正在运行的容器：`docker ps`
* 删除container:  `docker rm -f bioinfo_tsinghua`

## Semester Plan
### 编程技能
1. **目标**：
	- 学习利用Linux系统进行生物信息学操作。
    - 熟练掌握R的基础知识和高级特性，若有需要温习Python并加以应用
2. **学习内容与安排**：
    - Linux：复习基础（Week: 1）+随课程学习（Week: 2-5）
    - R+Python: 学习R基础(Week: 2-5)+随课程学习（Week: 6-16）
### NGS数据分析
1. **目标**：
    - 了解常见NGS相关软件及操作方法。
    - 掌握NGS数据处理和分析的基本方法，尽可能与个人实验室项目相结合应用学习。
2. **学习内容与安排**
    - 基本软件与数据处理操作：随课程学习（Week: 4-11）
    - 尝试使用NGS数据集进行实际分析，完成一些基于NGS数据的小型项目或练习：随学习进度而定
### 机器学习
1. **目标**：
    - 了解机器学习的常用算法与模型。
    - 尝试应用机器学习解决实际问题，尽可能与个人实验室项目相结合。
2. **学习内容与安排**：
    - 学习机器学习的基本原理、算法、模型：随课程学习（Week 12-16）
    - 尝试完成一些生物信息学的机器学习项目，如有可能进行蛋白质结构预测：随学习进度而定
