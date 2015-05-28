# taxperson
3 - Taxperson

public int totalCost(int merchandiseCost, int merchandiseType) {     int taxRate;     if (merchandiseType == Type.luxury)     {          taxRate = Tax.luxury;     }     else if (merchandiseType == Type.necessary)     {          taxRate = Tax.necessary;     }     else     {         throw new WrongTypeException("No such mechandise type");     }      retrun   merchandiseCost * (1 +  taxTate); }    public class WrongTypeException extends Exception {       public WrongTypeException(String message)      {          super(message);      } }  public class Type {    public static luxury = 1;    public static necessary = 2; } public class Tax {    public static luxury = 0.09;    public static necessary = 0.01; }
 
