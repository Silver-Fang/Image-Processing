埃博拉酱的图像处理工具包，提供一系列 MATLAB Image Processing Toolbox 内置函数所欠缺，但却常用的图像处理功能。

本包中所有函数均在ImageProcessing命名空间下，使用前需import。使用命名空间是一个好习惯，可以有效防止命名冲突，避免编码时不必要的代码提示干扰。
```MATLAB
import ImageProcessing.*
```
函数文件内有详细文档，可用doc命令查看。
```MATLAB
%内置imwarp的升级版，支持3D图像批量变换
function varargout=ImWarp(Image,varargin)
%内置normxcorr2的升级版，支持多图批量操作
function C=NormXCorr2(template,A,Partial)
%对NormXCorr2的模板进行预处理
function FDN = Nxc2TPreprocess(Template,SizeA)
%使用Nxc2TPreprocess的预处理结果计算NormXCorr2
function C = Nxc2APostprocess(A,SizeT,FDN,Partial)
```