<div align="center">
<h1 align="center">体温上报助手</h1>
</div>


## 简介

自动完成每日体温上报 。

**如果当日有异常，请手动在小程序端/PC 端填写！！！！！！！！！！！！**

## Github Actions 启用步骤


### 1. Fork 本项目

Fork 本项目: [zhangt2333/actions-SduHealthReport](https://github.com/zhangt2333/actions-SduHealthReport) (Star 自然是更好)

### 2. 准备需要的参数

```
{
    # fill them:
    'username': 'fill-it',  # 学号
    'password': 'fill-it',  # 密码
    'ZXSJ': 'fill-it',  # 手机
    'XM': 'fill-it',  # 姓名
    'XSXB': 'fill-it',  # 性别, 填 '男' 或 '女'
    'NL': 'fill-it',  # 年龄
    'FDYXMX': 'fill-it',  # 辅导员姓名
    'SZDW': 'fill-it',  # 学院全称, 如 计算机科学与技术学院
    'ZYMC': 'fill-it',  # 专业全称, 如 计算机科学与技术（菁英班）
    'JJLXRXM': 'fill-it',  # 家长姓名
    'JJLXRDH': 'fill-it',  # 家长手机
    'JJLXRYBRGX': 'fill-it',  # 和家长关系, 如 父子
    'sheng': 'fill-it',  # 省, 如 山东省
    'shi': 'fill-it',  # 市, 如 青岛市
    'quxian': 'fill-it',  # 区/县, 如 即墨区
    'DQJZDZ': 'fill-it',  # 具体地址, 如 山东省青岛市即墨区鳌山卫街道滨海路72号
    'EXTEST': '否No',  # 是否进行过核酸和血清抗体检测, 填 '否No' 或 '是Yes'

    # choose once, then annotate others:
    'DQSFJJIA': '在家At home',
    # 'DQSFJJIA': '在外Away from home',

    # choose once, then annotate others:
    'LXZT': '非学校所在城市Not in the city of the university',
    # 'LXZT': '学校所在城市In the city of the university',
    # 'LXZT': '境外Abroad',
}
```

### 3. 启用 Github Actions

![image-20210216140844300](README/image-20210216140844300.png)

### 4. 将参数填到 Secrets

将填好的参数加入到 Secrets 中，name 为 `DATA`，value 为步骤 2 中的多行字符串

![image-20210216140557947](README/image-20210216140557947.png)