---
title: Unity-NavMesh
author: lihaoming
date: 2023-04-26 10:23:00 +0800
categories: [Unity, NavMesh]
tags: [Unity]
---

# NavMesh

## NavMeshPath
获取方法:
NavMesh.CalculatePath: 静态方法，传入起始点和终点，即可计算出路径角点。
NavMeshAgent.CalculatePath: 传入终点，将会根据agent对象的信息，计算出路径角点。
状态status:
PathComplete: 可到达
PathPartial: 只有一部分的路径
PathInvalid: 没找到路径
角点corners:
返回的角点坐标，忽略了导航网格高度的变化。如果想要获取准确的路径需要以水平面上的坐标插值为起点，使用射线命中的方式获取导航网格上具体的点位。



