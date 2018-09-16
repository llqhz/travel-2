lex 布局总结
display: flex/inline-flex;  指定弹性布局

主轴方向
flex-direction: row | row-reverse | column | column-reverse;
                左右      右左        上下       下上
主轴换行
flex-wrap: nowrap | wrap | wrap-reverse;
           1-->2  1->/2->   2->/1->         1-> 表示第一行  / 表示换行

主轴延展:  flex-flow: <flex-direction> || <flex-wrap>;  简洁语法同时定义主轴方向和换行
( 主轴方向 + 主轴换行 )

主轴项目聚集地方 ( 多个项目的聚集地方 )
justify-content: flex-start | flex-end | center | space-between | space-around;
                  聚左         聚右       聚中     顶两端分散      均匀侧距分散

  space-around:     ---[ ]------[ ]------[ ]---       顶端的margin会比中间的小一倍
                   ---[ ]---|---[ ]---|---[ ]---       ( 均匀侧距分散 )

叉轴项目对齐线 ( 各单个项目的对齐线 )
align-items: flex-start | flex-end | center | baseline | stretch;
             上对齐        下对齐     居中     基线      拉伸占满


多横轴聚集地方 ( 多条线聚集地方 )
align-content: flex-start | flex-end | center | space-between | space-around | stretch;
                 聚上         聚下     聚中      顶两端分散    均匀侧距分散    均匀拉伸


----------------------
项目上的属性
----------------------

order: <integer>;   调整项目顺序
flex-grow: 0|<number>;   剩余空间的分配权重 | 项目放大比例
flex-shrink: 1|<number>; 项目的缩小比例  空间不足，项目允许缩小。
flex-basis: auto|<length>;   flex项目宽度
[ 合写 ]
flex: flex-grow | flex-shrink | flex-basis

align-self: auto | flex-start | flex-end | center | baseline | stretch;
    垂直对齐方式: 覆盖align-items


-----------------------------------------
| 父: 主轴延展方向,主叉轴的对齐聚集方向 |
| 子: 伸缩权重,宽度,对齐方式            |
-----------------------------------------
