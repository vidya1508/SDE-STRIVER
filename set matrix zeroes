class Solution {
    public void setZeroes(int[][] matrix) {
        //rows
        int row=matrix.length;
        int col=matrix[0].length;
        //flag varibles to take care of 1st row and second row
        boolean rowfill=false;
        boolean colfill=false;
        //now the part 1 of game starts: if row has zeroes
        for(int i=0;i<col;i++)
        {
            if(matrix[0][i]==0)
            {
                rowfill=true;
                break;
            }
        }
        //find if col has any zeroes
        for(int i=0;i<row;i++)
        {
            if(matrix[i][0]==0)
            {
                colfill=true;
            }
        }
        //now the interesting part: TREASURE HUNT HAHAHHA
        for(int i=1;i<row;i++)
        {
            for(int j=1;j<col;j++)
            {
                if(matrix[i][j]==0)
                {
                    matrix[i][0]=0;
                    matrix[0][j]=0;
                }
            }
        }
        //use the treasure to make it clear
        for(int i=1;i<row;i++)
        {
            for(int j=1;j<col;j++)
            {
                if(matrix[i][0]==0|| matrix[0][j]==0)
                {
                    matrix[i][j]=0;
                }
            }
        }
        // don't be a fool and complete what you've started
        if(rowfill)
        {
            for(int i=0;i<col;i++)
            {
                matrix[0][i]=0;
            }
        }
         if(colfill)
        {
            for(int i=0;i<row;i++)
            {
                matrix[i][0]=0;
            }
        }

        
    }
}
