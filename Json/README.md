### Example


```c
#include <stdio.h>
#include "json.h"

int main(void)
{

    unsigned char age = 0;
    char name[20] = "";

    char json[200] = "{\"name\":\"Jonas Vargaski\",\"age\":25}";

    getString(json, "name", name);
    age = getInt(json, "age");

    printf("name: %s \r\nage: %d\r\n", name, age);
    return 0;
}
```