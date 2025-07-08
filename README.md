# -DATA-COMPRESSION-TOOL

*COMPANY NAME* : CODTECH IT SOLUTIONS

*NAME* : PUNEET VASHISTH

*INTERN ID* : CT04DG757

*DOMAIN* : C PROGRAMMING

*DURATION* : 4 WEEKS

*MENTOR* : NEELA SANTOSH

*I USE VS CODE*

THE CODE IS 

#include <stdio.h>
#include <string.h>

void runLengthEncode(const char *input) {
    int len = strlen(input);
    int count = 1;

    for (int i = 0; i < len; i++) {
        // Count occurrences of the same character
        while (i < len - 1 && input[i] == input[i + 1]) {
            count++;
            i++;
        }

        // Print character followed by count
        printf("%c%d", input[i], count);
        count = 1;
    }
    printf("\n");
}

int main() {
    char input[1000];

    printf("Enter a string to compress: ");
    scanf("%s", input); // Note: reads up to whitespace

    printf("Compressed Output (RLE): ");
    runLengthEncode(input);

    return 0;
}
VS CODE OUT PUT IS 

<img width="257" height="192" alt="Image" src="https://github.com/user-attachments/assets/cd128c07-b0b8-4ed2-ae52-9d57ff7f7c62" />
