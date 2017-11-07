# Assignment003
package Problem001;

public class Matrix{
int rows;
int cols;
double[][] elements;
Matrix original;
double[][] element;

public Matrix(Matrix original) {
	this.original = original;
}

public Matrix(int rows, int cols) {
	this.rows=rows;
	this.cols=cols;
	elements = new double[rows][cols];
}
public Matrix(double[][] elements){
	rows=3;
	cols=3;
this.elements = new double[rows][cols];
    for (int i = 0; i < rows; i++)
        for (int j = 0; j < cols; j++)
                this.elements[i][j] = elements[i][j];
}


public Matrix add(Matrix other) {
Matrix result = new Matrix(rows,cols);//Im not sure why...i looked it up
	for(int i = 0; i<rows;i++)
		for(int j=0;j<cols;cols++) 
			original.element[i][j] + other[i][j]= result[i][j];
	return result; 
}


public Matrix sub(Matrix other) {
	Matrix result = new Matrix(rows,cols);//Im not sure why...i looked it up
	for(int i = 0; i<rows;i++)
		for(int j=0;j<cols;cols++) 
			original.element[i][j] - other[i][j]= result[i][j];
	return result;
}

public Matrix elementMulti1(Matrix other) {
	Matrix result = new Matrix(rows,cols);//Im not sure why...i looked it up
	for(int i = 0; i<rows;i++)
		for(int j=0;j<cols;cols++) 
			original.element[i][j] * other[i][j]= result[i][j];
	return result;
	
}

public Matrix multi(Matrix other) {
	
}

public Matrix opposite() {
	public Matrix elementMulti(Matrix other) {
		Matrix result = new Matrix(rows,cols);//Im not sure why...i looked it up
		for(int i = 0; i<rows;i++)
			for(int j=0;j<cols;cols++) 
				original.element[i][j] * other[i][j]*-1= result[i][j];
		return result;
}

public Matrix transpose() {
	
}

public double determinant() {
	double determ;
	double a=original.element[1][1];
	double b=original.element[1][2];
	double c=original.element[1][3];
	double d=original.element[2][1];
	double e=original.element[2][2];
	double f=original.element[2][3];
	double g=original.element[3][1];
	double h=original.element[3][2];
	double i=original.element[3][3];
determ = Math.abs((a*(e*i-f*h)-b*(d*i-f*g)+c*(d*h-e*g)));
	return determ;		
}

public String toString() {
	
}

public static void main(String[] args) {
	
}	
}//end class
