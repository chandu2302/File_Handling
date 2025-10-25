//# File_Handling
//The program ensures only authorized users can access or modify the file content

#include <stdio.h>
#include <string.h>
#include "Types.h"
void main(int argc, char** argv)
 {
    char password[7] = "abc123", user_pass[7];
    if(argc != 4) 
  	{	
		printf(“enter password\n”);
		return;
		}
    printf("Enter password: ");
    scanf("%s", user_pass);
    if(strcmp(user_pass, password) != 0)
		{
		printf(“Incorrect password\n”);
		 return;
		}
    if(strcmp(argv[1], "-e") == 0)
		{
        encrypt_decrypt(argv[2], argv[3], password);
    	}else{
        encrypt_decrypt(argv[2], argv[3], password);
          printf(“Successful\n”);
	 }
}<img width="486" height="874" alt="image" src="https://github.com/user-attachments/assets/fe4e0fae-49ce-4217-a6e1-7b56efc03782" />
