 #include <iostream>
 #include <fstream>
 #include <cstdlib>
 #include <iomanip>
 #include <cctype>
 
 using namespace std;
 
 int main ()
{
    ifstream fin, fin2;
    ofstream fout, foutA, foutB;
    
    fin.open("gba.txt");
    fin2.open("gba.txt");
    fout.open("result.txt");
    foutA.open("uppercase.txt");
    foutB.open("capitalize.txt");
    
    string words, spacedWords;
    double countWords = 0;
    double numChars = 0;
    double average;
    int strLength;
    int strLength1 = 0;
    int strLength2 = 0; 
    int strLength3 = 0; 
    int strLength4 = 0; 
    int strLength5 = 0;
    int strLength6 = 0;
    int strLength7 = 0; 
    int strLength8 = 0;
    int strLength9 = 0; 
    int strLength10 = 0;
    int strLength11 = 0; 
    int i = 0;
    
    if (fin.fail())
    {
        cout << "error opening input file" << endl;
        exit(1);//exit from program, go back it was not successful
    }
    if (fout.fail())
    {
        cout << "error with output file" << endl;
        exit(1);//exit from program, go back it was not successful
    }
    
    //loop that intakes the data from file
    while (!fin.eof()) 
    {
        fin >> words;
        countWords++;
        numChars += words.length();
        
        //Capitalizing the first letter of each word
        spacedWords = words + " ";
        
        if (spacedWords[i] > 90)
        {
            spacedWords[i] = int(spacedWords[i]) - 32;
        }
        foutA << (spacedWords[i]) + spacedWords.substr((i + 1), spacedWords.length()) << endl;
        
        //Capitalizes everything
        for ( int ix = 0; ix < words.length(); ix++)
        {
            char capitalizedWords;
            string word = "";
            capitalizedWords = toupper(words[ix]);
            word += capitalizedWords;
            foutB << word;
        }
        foutB << " ";
        
        //Switch statement that checks the length of the words
        switch (strLength)
        {
            case 1: strLength1++; 
            break;
            
            case 2: strLength2++;
            break;
            
            case 3: strLength3++;
            break;
            
            case 4: strLength4++;
            break;
            
            case 5: strLength5++;
            break;
            
            case 6: strLength6++;
            break;
            
            case 7: strLength7++;
            break;
            
            case 8: strLength8++;
            break;
            
            case 9: strLength9++;
            break;
            
            case 10: strLength10++;
            break;
            
            case 11: strLength11++;
            break;
            
       } 
        //cout << words << endl;
        
    }
   
            
    //cout << "Number of words in the text: " << countWords << endl;
    //cout << numChars << "/" << countWords << "=" << average << endl;
    average = numChars/countWords;
    fout << "Average characters per word: " << average << endl;
    fout << "Number of words in the text: " << countWords << endl;
    fout << "There are " << strLength1 << " words with a length of 1 char.\n" << "There are " << strLength2 << " words with a length of 2 chars.\n" << "There are " << strLength3 << " words with a length of 3 chars.\n" << "There are " << strLength4 << " words with a length of 4 chars.\n" << "There are " << strLength5 << " words with a length of 5 chars.\n" << "There are " << strLength6 << " words with a length of 6 chars.\n" << "There are " << strLength7 << " words with a length of 7 chars.\n" << "There are " << strLength8 << " words with a length of 8 chars.\n" << "There are " << strLength9 << " words with a length of 9 chars.\n" << "There are " << strLength10 << " words with a length of 10 chars\n." << "There are " << strLength11 << " words with a length of 11 chars.\n";
    fin.close();
    fin2.close();
    fout.close();
    foutA.close();
    foutB.close();
    
    return 0;
}
    
    
 
