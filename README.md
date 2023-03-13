# PSO-based-drone-movement

无人控制巡飞弹群，根据临近无人机的搜索获得打击目标。

% 参数介绍

N = 10;             % 无人机数目
maxiter = 100;      % 最大迭代次数----通信能力为基础的
w = 0.8;            % 无人机的速度惯性
c1 = 1.0;           % 周边无人机位置的解算参数
c2 = 1.4;           % 目标位置的解算参数

target = [1000, 1000, 500];% 目标坐标



% 2.0目标

目标target设置为矩阵，对多目标进行排序。当eps=10^(-6)时，释放一个无人机进行打击。
