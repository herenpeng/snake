# 贪吃蛇小游戏

一个基于 `JavaScript` 的网页版贪吃蛇小游戏。

<p align="center">
	<a target="_blank" href='https://gitee.com/herenpeng/snake'>
		<img src='https://gitee.com/herenpeng/snake/badge/star.svg' alt='gitee star'/>
	</a>
	<a target="_blank" href='https://github.com/herenpeng/snake'>
		<img src="https://img.shields.io/github/stars/herenpeng/snake.svg?logo=github" alt="github star"/>
	</a>
</p>
<hr/>

<br/>

## 游戏开始

使用浏览器打开 `snake.html` 文件，可以看到小游戏的主界面。

![游戏开始](./img/01.png)

按下键盘回车键，即可开始游戏，使用键盘的上、下、左、右四个方向键，即可控制贪吃蛇移动。

![选择方向](./img/02.png)

## 游戏暂停

在游戏中，重新按下回车键，即可暂停游戏。

![游戏暂停](./img/03.png)

## 游戏参数

### 迷宫大小

`snake.html` 文件中的常量 `MAX_HIGH` 和 `MAX_WIDE` 分别控制迷宫的高度和宽度，可以通过修改这两个值直接修改迷宫的大小，无需修改游戏逻辑。

### 游戏模式

游戏一共有两种模式：

- 正常模式：该模式中迷宫墙体为真实墙体，贪吃蛇触之即死。

- 无限模式：该模式下迷宫墙体为时空间隙，贪吃蛇撞墙后，会从墙体的另一边穿越过来。

游戏模式可以通过修改 `snake.html` 文件中的 `CYCLE` 布尔常量值来修改。

| 模式 | CYCLE |
| --- | --- |
| 正常模式 | false |
| 无限模式 | true |

### 其他参数

蛇身颜色，蛇身初始化位置、方向、长度，食物颜色，迷宫背景颜色等等都可以通过修改源码内定义的参数来实现。

## 游戏死亡

| 模式 | 死亡原因 |
| --- | --- |
| 正常模式 | 撞墙、咬到自己的身体 |
| 无限模式 | 咬到自己的身体 |

![游戏死亡](./img/04.png)

## 重新开始

在任意情况下，只要按下键盘 F5 键，即可刷新网页小游戏，重新开始。
