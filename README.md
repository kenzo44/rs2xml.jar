# rs2xml.jar
Was working on Java program for class and had to retrieve information from a database and populate it into a table. Thought someone else might need this. Just download the jar file and configure the path to you project.


Populate JTable with data from any database...

  	Connection con = getConnection();

  	PreparedStatement statement = con.prepareStatement("SELECT * FROM table");
					
	ResultSet rs = statement.executeQuery();
					
	displayTable.setModel(DbUtils.resultSetToTableModel(rs));
