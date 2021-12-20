#include <stdio.h>
#include <string.h>

int main()
{

    char data[100];


    //file pointer variable
    FILE *fxpmptr;
    FILE *fxpmptr2;
    FILE *fxpmptr3;

    //point pointer variable to file
    fxpmptr = fopen("C:\\Users\\user\\Desktop\\beforetest.txt","r");
    fxpmptr2 = fopen("C:\\Users\\user\\Desktop\\beforetest.xpm","w");
    fxpmptr3 = fopen("C:\\Users\\user\\Desktop\\aftertest.xpm","w");


    while(!feof(fxpmptr)){
        fscanf(fxpmptr,"%[^\n] ",data);


        char* token = strtok(data, "#");


        while(token!=NULL)
        {

            if(strcmp(token,"2faf49")==0)
            {
                fprintf(fxpmptr2,"#%s",token);
                fprintf(fxpmptr3,"#1f4677");

            }
            else if(strcmp(token,"bb1c2a")==0)
            {
                fprintf(fxpmptr2, "#%s", token);
                fprintf(fxpmptr3, "#f48d79");
            }
            else if(strcmp(token,"9337d0")==0)
            {
                fprintf(fxpmptr2,"#%s",token);
                fprintf(fxpmptr3,"#d5bbfe");
            }
            else{
                fprintf(fxpmptr2,"%s",token);
                fprintf(fxpmptr3,"%s",token);
            }

            token = strtok(NULL, "#");

        }
        fprintf(fxpmptr2,"\n");
        fprintf(fxpmptr3,"\n");

    }

    //close file
    fclose(fxpmptr);
    fclose(fxpmptr2);
    fclose(fxpmptr3);

    return 0;
}

