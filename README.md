# Ini File Libraries
A library for read and write Initialization file based on the Windows API.

## Usage

```cpp
#include "Ini.h"
using namespace Easy;

CString sPath = _T("D:\\config.ini");

Ini ini(sPath);

int nValue = 0;
bool bValue = false;
CString sValue;

ini.Read(_T("Setting"), _T("Key1"), nValue);
ini.Read(_T("Setting"), _T("Key2"), bValue);
ini.Read(_T("Setting"), _T("Key3"), sValue);

ini.Write(_T("Setting"), _T("Key1"), nValue);
ini.Write(_T("Setting"), _T("Key2"), bValue);
ini.Write(_T("Setting"), _T("Key3"), sValue);

```
