# hfs_for_oss
HTTP File Server for AliYun OSS  
A modern HTTP File Server for oss@aliyun.  
һ���ִ�����http�ļ���������Ϊ������OSS����洢�����ṩ֧�֡� 
  
SDK��[aliyun-oss-php-sdk](https://help.aliyun.com/document_detail/32101.html?spm=5176.doc52834.6.753.ihtpJC)-2.2.4�ṩ��������[h5ai](https://larsjung.de/h5ai/)�ṩ��

## Ԥ�� & ����/Demo & Download
* Ԥ����http://file.oovoo.site/
* ���أ�https://github.com/YuXuan220/hfs_for_oss/releases

## ����/Build
* ����Ҫ��  
PHP 5.5�����ϣ�û��֤�ݱ��������޷���PHP5.5�����������У�
* �ļ��ṹ��
```
/
������aliyun-oss-php-sdk-2.2.4/	--SDKĿ¼
  ������src/
    ������...
  ������autoload.php
  ������common.php
������h5ai/	--h5Ŀ¼
  ������css/
    ������style.css  --���Զ����css
  ������images/
    ������...
  ������js/
    ������...
������config.php	--�����ļ�
������get_files.php	--listObjects(), ��ȡ�ļ��б�
������index.php	--��ҳ
```
* ���ã�   
~~~php
/config.php: 
<?php  
final class Config  
{  
	const OSS_ACCESS_ID = '';   //Access Key ID  
	const OSS_ACCESS_KEY = '';    //Access Key Secret  
	const OSS_ENDPOINT = ''; //OSS EndPoint (e.g. http://oss-cn-shanghai.aliyuncs.com)  
	const OSS_BUCKET = ''; //OSS Bucket Name  
}  
$site = '' ;   //Site Name  
$footer = '';   //Footer, Stats Code Supported  
$stats = true ;    //Display how long listObjects() takes? (true/false)  
~~~

## �������ܵĸĶ�/Preview
```
[�޸�] ·���㼶��ĳһ��������һ���ļ���������ʾ������
[����] ���item�Ĵ�С
[����] �Ϸ�crumbbar·���༶��ʾ����������ַ����˳�path���ÿһ��·����ĺ��鷳��������"../"�ͺ��˰���Ҳ�ܾ�������
[����] �򵥵�object�����ܣ��ϴ����������ȣ�
[��Զ�������еĹ���\]��������˼��������ǹ��ź��Ƶ�΢Ц���� �ļ��б�����
```

## ������־/ChangeLog
```
version 1.0.0 2017-06-17
	�ƿǡ�
```

## ��ԴЭ��/License
����Ȼ�Һ�����WTFPL������Ц~����
```
The MIT License (MIT) 
 
Copyright (c) 2016 Lars Jung (https://larsjung.de)

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
```