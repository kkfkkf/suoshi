
    tar_replacefile.bat脚本用于在windows电脑上，对java项目的替换文件进行批量打包
	
	使用方法：
	1、配置patch_file.txt文件

		1）patch_file.txt文件的第一行是本机java项目的工程路径，例如：
			D:\software\apache-tomcat-7.0.54-1\webapps\web\
			
		2）patch_file.txt文件的第二行到最后一行是替换文件的绝对路径，例如：
			D:\software\apache-tomcat-7.0.54-1\webapps\web\WEB-INF\classes\com\fh\iasp\app\cm\v2\dao\BasCmCusStoreDao.class
			D:\software\apache-tomcat-7.0.54-1\webapps\web\WEB-INF\classes\com\fh\iasp\platform\pojo\AppMenu.class
			D:\software\apache-tomcat-7.0.54-1\webapps\web\app\blog\web\v8\include_weibo.jsp
			
	
	2、双击运行tar_replacefile.bat脚本
	
		1）输入项目名称
			为了方便区分，每次打包，需要输入项目名称，例如：
				1>如果是【高级拜访】功能，则输入customer_visit；
				2>如果是appsvr平台的，则输入appsvr；
				3>如果是多个应用模块的，则输入appsvr；
				
		2）在当前路径获取压缩包，提交jira