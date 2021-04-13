//Вариант3 средний уровень
//В заданной строке каждую русскую букву заменить на символ" *"
#include <iostream>
#include <string>
#include <regex>
using namespace::std;


int main()
{
    setlocale(LC_ALL, "Russian");
    wstring s = L"hellow world господа da da da";
    wcout << "s= " << s << endl;
    s = regex_replace(s, wregex(L"[а-я,А-Я]"), wstring(L"*"));
    wcout << "s= " << s << endl;
    system("pause");
    return 0;
}
