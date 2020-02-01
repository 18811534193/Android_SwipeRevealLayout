# Android_SwipeRevealLayout
安卓侧滑删除、分享

添加
<？xml版本=“ 1.0”编码=“ utf-8”？>
<android.support.constraint.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context="com.rock.han.sideslipstudy.MainActivity">

<LinearLayout
    android:orientation="vertical"
    android:layout_width="match_parent"
    android:layout_height="match_parent">
    <com.chauthai.swipereveallayout.SwipeRevealLayout
        android:id="@+id/swipe_layout_1"
        android:layout_width="match_parent"
        android:layout_height="70dp"
        android:layout_margin="10dp"

        app:mode="normal"
        app:dragEdge="right">

        <LinearLayout
            android:layout_width="wrap_content"
            android:layout_height="match_parent"
            android:orientation="horizontal">

            <TextView
                android:layout_width="70dp"
                android:layout_height="match_parent"
                android:gravity="center"
                android:background="@android:color/darker_gray"
                android:textColor="@android:color/white"
                android:text="More"
                android:onClick="moreOnClick"/>

            <TextView
                android:layout_width="70dp"
                android:layout_height="match_parent"
                android:gravity="center"
                android:background="@android:color/holo_red_dark"
                android:textColor="@android:color/white"
                android:text="Delete"
                android:onClick="deleteOnClick"/>
        </LinearLayout>

        <FrameLayout
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:background="#ffffff"
            android:onClick="layoutOneOnClick">

            <TextView
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:text="My Awesome Layout 1"
                android:gravity="center"
                android:layout_gravity="center"/>
        </FrameLayout>
    </com.chauthai.swipereveallayout.SwipeRevealLayout>




    <TextView
        android:text="ListView侧滑"
        android:layout_width="match_parent"
        android:layout_height="wrap_content" />
    <ListView
        android:id="@+id/list_view"
        android:background="@color/colorPrimary"
        android:layout_width="match_parent"
        android:layout_height="200dp"
        android:divider="@null"/>

    <TextView
        android:text="——————————"
        android:layout_width="match_parent"
        android:layout_height="wrap_content" />
    <TextView
        android:text="RecyclerView侧滑"
        android:layout_width="match_parent"
        android:layout_height="wrap_content" />
    <android.support.v7.widget.RecyclerView
        android:background="@color/colorAccent"
        android:id="@+id/recyclerView"
        android:layout_width="match_parent"
        android:layout_height="200dp" />
</LinearLayout>
</android.support.constraint.ConstraintLayout>
