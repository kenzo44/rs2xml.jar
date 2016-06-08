# rs2xml.jar

Populate JTable with data from any database...

  Connection con = getConnection();

  PreparedStatement statement = con.prepareStatement("SELECT * FROM table");
					
	ResultSet rs = statement.executeQuery();
					
	displayTable.setModel(DbUtils.resultSetToTableModel(rs));
