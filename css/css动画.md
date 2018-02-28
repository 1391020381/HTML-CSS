# CSS中动画类型<chrome F12  ESC  左侧的三个圆点可以选择动画面板 >
1. transition 补间动画(元素的状态,需要有变化<hover 添加class>)
2. keyframe关键帧动画 animation
   * animation-direction:reverse
   * animation-fill-mode:forwards<保持动画的最终值>  backwards
   * animation-iteration-count:infinite
   * animaiton-play-state:paused
   * animation-timing-function:steps(1)  时间和动画间关系<steps指定关键帧间的补间> 
3. 逐帧动画
* [cubic-bezier](http://cubic-bezier.com/#.17,.67,.83,.67)
# CSS动画性能
 1. 性能不坏
 2. 部分情况下优于js
 3. 但js可以做的更好
 4. 部分高危属性  box-shadow等  有影阴的