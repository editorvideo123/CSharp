# CSharp
此存储库包含有关 C# 的各种内容

这是使用 C# 语言创建 ASP Dotnet Core 项目的命令
dotnet new web --name latihan2 --language C#

您需要创建一个 wwwroot 文件夹来放置网页文件


下面是测试连接MariaDB数据库的源码

```

using System;

using MySql.Data.MySqlClient;

namespace file2{
	
	
	class program3{
		
		
		static void Main(string[]args){
			
			string koneksiString = null;
			
			MySqlConnection koneksi;
			
			koneksiString = "server=1.1.3.8;database=latihan;uid=steven;password=kucing;";
			
			koneksi = new MySqlConnection(koneksiString);
			
			
			try{
				
				
				koneksi.Open();
				
				Console.WriteLine("Berhasil Terkoneksi Ke Server");
				
				koneksi.Close();
			}
			
			catch(Exception ex){
				
				Console.WriteLine("Gagal Terhubung Ke Server");
			}
			
			
		}
	}
	
	
}

```

我正在尝试了解 Kestrel 服务器在 C# 中的用法，以便稍后在 ASP .NET 和 Blazor 中使用。我还需要了解 Razor 页面












