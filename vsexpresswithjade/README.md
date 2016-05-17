# vsexpresswithjade

如何使用typescript
1.安裝工具或是手動下載
	a.tsd
	b.typings
	c.nuget
2.由於這裡是用typings所以只說明如何使用typings
  到Scripts的資料夾下使用cmd。
3.輸入typings install <moduleName> (--ambient在某些情況下需要) --save
4.會產生main(server)跟browser(client)兩個資料夾。
5.到tsconfig.json利用exculde的功能將不需要的資料夾排除。
6.使用建置(build)如果出現"Promise not found"，
  就表示需要到tsconfig.json中將'target'設成'es6'。
  (因為有用到es6的東西?lib.es6)