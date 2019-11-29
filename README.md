# HSwipeRefreshLayout
```
//用法与原生一致
mSwipeRefresh = mBinding.shrlLayout;

if (mBinding.getRoot().getContext() != null) {
  final TypedArray typedArray = getContext().obtainStyledAttributes(
          new int[]{R.attr.color_mgo_common_refresh, R.attr.color_mgo_common_bg});
   mSwipeRefresh.setColorSchemeColors(typedArray.getColor(0, Color.WHITE));
   mSwipeRefresh.setProgressBackgroundColorSchemeColor(typedArray.getColor(1, Color.WHITE));
}

mSwipeRefresh.setOnRefreshListener(this::onRefresh);
mSwipeRefresh.setRefreshing(false);
mSwipeRefresh.setRefreshing(true);
```