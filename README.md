# BigData

	BigData(INT64 data);
	BigData(const char *str);
	BigData operator+(BigData& d);
	BigData operator-(BigData& d);
	BigData operator*(BigData& d);
	BigData operator/(BigData& d);
	friend string Add(string& left, string& right);
	friend string Sub(string& left, string& right);
	friend string Mul(string& left, string& right);
	friend string Div(string& left, string& right);
	bool _IsINT64OverFlow()const;//判断数据是否溢出
	friend ostream& operator<<(ostream& _cout, const BigData& d);//重载输出流运算符
	void _INT64ToString();//将INT64类型转换为string类型数据
