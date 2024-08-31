 class figure {
    double dim1;
     double dim2;

     public figure(double dim1, double dim2) {
        this.dim1 = dim1;
        this.dim2 = dim2;
    }


    public double area() {
        System.out.println("INSIDE FIGURE");
        return 0;
    }
}
class Rectangle extends figure {
    
    
    Rectangle(double dim1,double dim2) {
        super(dim1,dim2);
    
    }

public double area(){
    System.out.println("inside the area of rectangle");
    return dim1 * dim2;
}
}
class Triangle extends figure {
    Triangle(double dim1,double dim2) {
    super(dim1,dim2);
    
    }

public double area(){
    System.out.println("inside the area of Rectangle");
    return  0.15*dim1*dim2;
}
}

public class Usefigure{

public static void main(String[] s){
    figure t =new figure(30,10);
    
    Rectangle r =new Rectangle(9,5);
    t=r;
    System.out.println(t.area());
    Triangle tr= new Triangle(10,8);
    t=tr;
    System.out.println(t.area());
    
}

}
