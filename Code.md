Import java.sql.connection;
Import java.sql.DriverManager;
Import java.sql.ResultSet;
Import java.sql.SQLException;
Import java.sql.Statement;
Import java.util.logging.Level;
Import java.util.logging.Logger

Public class SchoolS{
boolean status = false;

Public static void main (string []args){
Connection connection = null;
Statement statement = null;
ResultSet resultset = null ;
try( Class.forName(“sun.jbdc.Jbdc0bcDriver”);
}Catch ( ClassNotFoundException ex) {
   Logger.getLogger( SchoolD.class.getName()).log(Level.SEVERE,null,ex);
}
try{
Connection = DriverManager.getConnection(“jdbc:odbc:ODBC School”);
Status = true;
}Catch (SQLException ex){
Logger.getLogger( SchoolD.class.getName()).log(Level.SEVERE,null,ex);
}
return status;
}
}

  
