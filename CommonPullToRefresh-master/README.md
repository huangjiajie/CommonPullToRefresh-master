# CommonPullToRefresh
Android widget with pull to refresh for all the views,and support loadMore for ListView,RecyclerView,GridView and SwipeRefreshLayout.

在[android-Ultra-Pull-To-Refresh](https://github.com/liaohuqiu/android-Ultra-Pull-To-Refresh)的基础上增加了加载更多的支持，感谢作者

* 下拉刷新支持大部分`view`：`ListView`、`ScrollView`、`WebView`等，甚至一个单独的`TextView`
* 加载更多目前支持`ListView`、`RecyclerView`、`GridView`、`SwipeRefreshLayout`
* 支持自定义header以及footer
* 增加SwipeRefreshLayout刷新方式，同样支持加载更多

#### 加载更多配置
* 是否需要加载更多
  默认`false`
  `mPtrFrame.setLoadMoreEnable(true)`
* 是否自动加载
  默认`true`
  `mPtrFrame.setAutoLoadMoreEnable(true)`

#### Header、Footer样式
* Header	实现接口`PtrUIHandler`，已有默认实现`PtrClassicDefaultHeader`，并通过`PtrFrameLayout.setHeaderView(View header)`设置
* Footer	实现接口`ILoadMoreViewFactory`，已有默认实现`DefaultLoadMoreViewFooter`，并通过`PtrFrameLayout.setFooterView(ILoadMoreViewFactory factory)`设置

## 常见问题

*  ViewPager滑动冲突: `disableWhenHorizontalMove()`
*  长按LongPressed, `setInterceptEventWhileWorking()`
*  如果要禁用下拉刷新，则更改`PtrHandler.checkCanDoRefresh`的返回实现即可



 

