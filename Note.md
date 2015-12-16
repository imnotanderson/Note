
[一个博客，路漫漫](http://www.lanindex.com/)

[GRPC](http://blog.csdn.net/q26335804/article/details/47616859)

4爷的博客 ugui
http://blog.csdn.net/u012091672/article/details/46876509

https://github.com/photonstorm/phaser

http://phaser.io/

http://cafebabe.cc/

Unity执行主菜单功能
EditorApplication.ExecuteMenuItem
q群关系
https://qun.insight-labs.org/

输入法禁止全屏
	
	View.setImeOptions(EditorInfo.IME_FLAG_NO_FULLSCREEN|EditorInfo.IME_ACTION_DONE);

安卓View偏移

	View CreateLayout(Context c,View cv)
	{
		RelativeLayout relativeLayout = new RelativeLayout(c);
		ViewGroup.LayoutParams lp = new ViewGroup.MarginLayoutParams(ViewGroup.LayoutParams.MATCH_PARENT, ViewGroup.LayoutParams.MATCH_PARENT);
		relativeLayout.setLayoutParams(lp);
		relativeLayout.addView(cv);
		//ChangeHeight(cv,360);
		return relativeLayout;
	}
	
	void ChangeHeight(View cv,int offset)
	{
		RelativeLayout.LayoutParams rp =(RelativeLayout.LayoutParams)cv.getLayoutParams();
		rp.bottomMargin = offset;
		rp.topMargin = -offset;
		cv.setLayoutParams(rp);
	}

===========================================================================
算法
http://blog.csdn.net/orbit/article/details/7082678
http://blog.csdn.net/orbit/article/details/7101869
逼近
http://blog.csdn.net/orbit/article/details/12793343
画直线
http://blog.sina.com.cn/s/blog_4a2183a60101dhr4.html
鱼群
http://blog.sina.com.cn/s/blog_4a2183a60101avwt.html
AABB相交
http://blog.sina.com.cn/s/blog_4a2183a601014vl3.html
计算几何
http://blog.sina.com.cn/s/blog_4a2183a601014tq6.html
三次平滑算法
http://blog.sina.com.cn/s/blog_4a2183a60100ymed.html
CatmullRom插值算法
http://blog.csdn.net/ym19860303/article/details/21401553
求贝赛尔 曲线的长度
http://blog.csdn.net/ym19860303/article/details/8277152
Dijkstra 算法原理
http://blog.csdn.net/ym19860303/article/details/8006217
四元数
http://blog.csdn.net/ym19860303/article/details/29572217
 Catmull–Rom样条插值
http://www.tuicool.com/articles/MJNNNvi
Cubic Hermite spline
https://en.wikipedia.org/wiki/Cubic_Hermite_spline#Catmull.E2.80.93Rom_spline
Cubic Hermite spline Github
https://github.com/nuhash/UnityCubicSpline/blob/master/CubicSpline.cs
=====================
http://www.element3ds.com/thread-40541-1-1.html
