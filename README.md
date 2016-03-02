# aliyun-mns
阿里云的官方mns sdk 的 composer 封装

# MNS SDK for PHP    
Please refer to http://www.aliyun.com/product/mns and  https://docs.aliyun.com/?spm=5176.7393424.9.6.5ki1hv#/pub/mns/api_reference/intro&intro for more API details.    

## Samples    
You must fulfill the AccessId/AccessKey/AccountID in the example before running.   

## Require
PHP >= 5.5

## Usage
Add the require_once("/path_to_sdk/mns-autoloader.php") in your php file when using sdk

## Usage as composer
just composer require aliyun/mns

```
"repositories": [
		{
			"type":"package",
			"package": {
				"name": "aliyun/mns",
				"version": "1.0.1",
				"source": {
					"type": "git",
					"url": "https://github.com/murdercdh/aliyun-mns.git",
					"reference": "master"
				},
				"autoload": {
					"files":[
						"src/GuzzleHttp/functions_include.php",
						"src/GuzzleHttp/Psr7/functions_include.php",
						"src/GuzzleHttp/Promise/functions_include.php"
					],
					"psr-4": {"AliyunMNS\\": "src/"}
				}
			}
		}
    ],
```