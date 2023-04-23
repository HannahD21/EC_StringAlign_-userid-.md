#include <iostream>
#include <string>

int main()
{
    std: :string str;
    int width;
    
    std: :cout << "Enter a string: ";
    std: :getline(std: :cin, str);
    
    std: :cout << "Enter width: ";
    std: :cin >> width;
    
    int len = str.length();
    int totalSpaces = width - len;
    
    char output[width];
    std: :fill(output, output + width, ' ');
    
    int spacesBefore = totalSpaces / 2;
    int spacesAfter = totalSpaces -
spacesBefore;
    
    int i = spacesBefore;
    for (char c : str)
    {
        output[i++] = c;
    }
    
    std: :cout << output << std: :end1;
    
    return 0;
}
