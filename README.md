# Vitas 
## 个人收藏的Android常用自定义控件。其主要功能有：
### 1.   AlignTextView
### 2.   CircleImageView
### 3.   SearchEditText
### 4.   ShapeTextView
### 5.   SwitchButtonView

# 集成AS   AndroidX
> Step 1.先在 build.gradle(Project:XXXX) 的 repositories 添加:

	allprojects {
		repositories {
			...
			maven { url "https://jitpack.io" }
		}
	}
> Step 2. 然后在 build.gradle(Module:app) 的 dependencies 添加:

	dependencies {
	
	        implementation 'com.github.zhangi789:Vitas:3.5.2'
	}
## AlignTextView

**1、两端对齐的TextView，可以设置最后一行靠左，靠右，居中对齐**

```xml
 <com.pandora.cn.widget.AlignTextView
        android:layout_width="match_parent"
        android:text="1.毋庸置疑四种"
        app:align="center"
        android:layout_height="wrap_content"/>
```

## CircleImageView

**1、 Android的圆形图像视图**

```xml
 <com.pandora.cn.widget.CircleImageView
              android:layout_width="160dp"
              android:layout_height="160dp"
              android:layout_centerInParent="true"
              android:src="@mipmap/wodetouxiang"
              app:civ_fill_color="@color/colorPrimary"
              app:civ_circle_background_color="@color/colorPrimaryDark"
              app:civ_border_width="1dp"
              app:civ_border_color="@color/colorAccent" />
```
## SearchEditText

**1、 android 自定义搜索框 支持自定义背景，游标颜色，支持更换搜索和删除图片**

```xml
 <com.pandora.cn.widget.SearchEditText
            android:id="@+id/searchEditText"
            android:layout_width="match_parent"
            android:layout_height="34dp"
            android:layout_margin="10dp"
            android:background="@drawable/search_edit_bg_rectangle"
            android:drawableLeft="@drawable/ic_search_gray"
            android:drawablePadding="0dp"
            android:textCursorDrawable="@drawable/search_edit_cursor_default"
            android:gravity="center_vertical"
            android:hint="请输入手机号"
            android:imeOptions="actionSearch"
            android:padding="5dp"
            android:singleLine="true"
            android:textSize="14sp"
            app:drawableDelete="@drawable/ic_clear" />
```
## ShapeTextView

**1、 自定义圆角矩形背景按钮，避免创建大量不可复用的shape.xml**

```xml
 <com.pandora.cn.widget.ShapeTextView
        android:id="@+id/mShapeTitleBar"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_gravity="center"
        android:layout_marginTop="30dp"
        android:gravity="center"
        android:lines="1"
        android:text="沉浸式标题栏"
        android:textSize="13sp"
        app:horizontalPadding="13dp"
        app:strokeWidth="1dp"
        app:tagColor="@color/colorPrimary"
        app:txtColor="@color/colorPrimary"
        app:verticalPadding="8dp" />

    <com.pandora.cn.widget.ShapeTextView
        android:id="@+id/mShapeAdapter"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_gravity="center"
        android:layout_marginTop="20dp"
        android:gravity="center"
        android:lines="1"
        android:text="适配器样式"
        android:textSize="13sp"
        app:fillType="normal"
        app:horizontalPadding="13dp"
        app:isRoundRect="true"
        app:pressedColor="#ffeee6"
        app:radius="20dp"
        app:strokeWidth="1dp"
        app:tagColor="@color/colorAccent"
        app:txtColor="@color/colorPrimary"
        app:verticalPadding="9dp" />


    <com.pandora.cn.widget.ShapeTextView
        android:id="@+id/mShapePop"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_gravity="center"
        android:layout_marginTop="20dp"
        android:gravity="center"
        android:lines="1"
        android:text="弹出框样式"
        android:textSize="13sp"
        app:fillType="normal"
        app:horizontalPadding="13dp"
        app:isRoundRect="true"
        app:pressedColor="#ffeee6"
        app:radius="20dp"
        app:strokeWidth="1dp"
        app:tagColor="@color/colorPrimary"
        app:txtColor="#ff5900"
        app:verticalPadding="9dp" />


    <com.pandora.cn.widget.ShapeTextView
        android:id="@+id/mShapeCustom"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_gravity="center"
        android:layout_marginTop="20dp"
        android:gravity="center"
        android:lines="1"
        android:text="自定义控件"
        android:textSize="13sp"
        app:fillType="fill"
        app:horizontalPadding="13dp"
        app:radius="20dp"
        app:strokeWidth="1dp"
        app:tagColor="@color/colorPrimaryDark"
        app:verticalPadding="9dp" />


    <com.pandora.cn.widget.ShapeTextView
        android:id="@+id/mShapeBanner"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_gravity="center"
        android:layout_marginTop="20dp"
        android:gravity="center"
        android:lines="1"
        android:text="轮播图演示"
        android:textSize="13sp"
        app:endTagColor="@color/colorAccent"
        app:fillType="fill"
        app:gradientType="true"
        app:horizontalPadding="13dp"
        app:radius="20dp"
        app:startTagColor="@color/colorPrimaryDark"
        app:strokeWidth="0dp"
        app:txtColor="#ffffff"
        app:verticalPadding="9dp" />
```

## SwitchButtonView

**1、 自定义SwitchButton 总有一款适合你**

```xml
  <com.pandora.cn.widget.SwitchButtonView
        android:id="@+id/switch_button"
        android:layout_gravity="center"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginTop="20dp"/>

    <com.pandora.cn.widget.SwitchButtonView
        android:layout_gravity="center"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginTop="20dp"
        app:sb_checked="true"/>


    <com.pandora.cn.widget.SwitchButtonView
        android:layout_gravity="center"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginTop="20dp"
        app:sb_show_indicator="false"
        app:sb_checked="true"/>

    <com.pandora.cn.widget.SwitchButtonView
        android:layout_gravity="center"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginTop="20dp"
        app:sb_checked_color="#fdc951"
        app:sb_checked="true"/>

    <com.pandora.cn.widget.SwitchButtonView
        android:layout_gravity="center"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginTop="20dp"
        app:sb_button_color="#db99c7"
        app:sb_shadow_color="#A36F95"
        app:sb_background="#FFF"
        app:sb_checkline_color="#a5dc88"
        app:sb_checked_color="#A36F95"
        app:sb_width="64dp"
        app:sb_height="30dp"
        app:sb_uncheckcircle_color="#A36F95"
        />

    <com.pandora.cn.widget.SwitchButtonView
        android:layout_gravity="center"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginTop="20dp"
        app:sb_enable_effect="false"/>
```


