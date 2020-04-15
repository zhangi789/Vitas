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
	
	        implementation 'com.github.zhangi789:Vitas:1.0'
	}
