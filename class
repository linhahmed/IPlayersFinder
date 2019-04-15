public class IP implements IPlayersFinder {
public static Point[] findPlayers(String[] photo, int team, int threshold) 
		{
			char ph[][] = new char [photo.length][photo[0].length()];
			int i,j;
			for(i=0;i<photo.length;i++)
			{
				for(j=0;j<photo[i].length();j++)
				{
					ph[i]=photo[i].toCharArray();
				}	
			}	
			int k,l,blocknums=0;
			int count=0; 
			int north = 0,east = 0,south = 0,west = 0;
			int minblock=threshold/4;
			 Point[] result= new Point[1000];
			for(i = 0; i < photo.length; i++)
			{
				 for(j = 0; j < photo[i].length(); j++)
				 {
					 if(Character.getNumericValue(ph[i][j])==team)
					 {
					  blocknums++;
					  ph[i][j]=' ';
					  //check east
					  if(j + 1 < photo[i].length())
				      {
						  for(k=j+1;k<photo[i].length();k++)
						  {
							  if(Character.getNumericValue(ph[i][k])==team)
							  {
								  if(east<=k)
								  {
									  east=k;
								  }  
								  blocknums++;
								  ph[i][k]=' ';
								  //check east
								  if(j + 1 < photo[i].length())
							      {
									  for(l=j+1;l<photo[i].length();l++)
									  {
										  if(Character.getNumericValue(ph[i][l])==team)
										  {
											  if(east<=l)
											  {
												  east=l;
											  }
											  blocknums++;
											  ph[i][l]=' ';
										  }  
									  }    
							      }
							      //Check west
							      if(j-1 >= 0)
							      {
							    	  for(l=j-1;l<=0;l--)
									  {
							    		  if(Character.getNumericValue(ph[i][l])==team)
							    		  {
							    			  if(west>=l)
							    			  {
							    				  west=l; 
							    			  }  
							    			  blocknums++;
							    			  ph[i][l]=' ';
										  } 
							          }
							      }
				                  //Check south
							      if(i + 1 < photo.length)
							      {
							    	  for(l=i+1;l<photo.length;l++)
									  {
							    		  if(Character.getNumericValue(ph[i][l])==team)
							    		  {
							    			  if(south<=l)
							    			  {
							    				  south=l;
							    			  }  
							    			  blocknums++;
							    			  ph[i][l]=' ';
										  } 
							          }
							      }
							      //Check north
							      if(i - 1 >= 0)
							      {
							    	  for(l=i-1;l<=0;l--)
									  {
							    		  if(Character.getNumericValue(ph[i][l])==team)
							    		  {
							    			  if(north>=l)
							    			  {
							    				  north=l;
							    			  }  
							    			  blocknums++;
							    			  ph[i][l]=' ';
										  } 
							          }
					              }
							  }  
						  }    
				      }
				      //Check west
				      if(j-1 >= 0)
				      {
				    	  for(k=j-1;k<=0;k--)
						  {
				    		  if(Character.getNumericValue(ph[i][k])==team)
				    		  {
				    			  if(west>=k)
				    			  {
				    				  west=k; 
				    			  } 
				    			  blocknums++;
				    			  ph[i][k]=' ';
				    			  //check east
								  if(j + 1 < photo[i].length())
							      {
									  for(l=j+1;l<photo[i].length();l++)
									  {
										  if(Character.getNumericValue(ph[i][l])==team)
										  {
											  if(east<=l)
											  {
												  east=l;
											  } 
											  blocknums++;
											  ph[i][l]=' ';
										  }  
									  }    
							      }
							      //Check west
							      if(j-1 >= 0)
							      {
							    	  for(l=j-1;l<=0;l--)
									  {
							    		  if(Character.getNumericValue(ph[i][l])==team)
							    		  {
							    			  if(west>=l)
							    			  {
							    				  west=l; 
							    			  }
							    			  blocknums++;
							    			  ph[i][l]=' ';
										  } 
							          }
							      }
				                  //Check south
							      if(i + 1 < photo.length)
							      {
							    	  for(l=i+1;l<photo.length;l++)
									  {
							    		  if(Character.getNumericValue(ph[i][l])==team)
							    		  {
							    			  if(south<=l)
							    			  {
							    				  south=l;
							    			  }
							    			  blocknums++;
							    			  ph[i][l]=' ';
										  } 
							          }
							      }
							      //Check north
							      if(i - 1 >= 0)
							      {
							    	  for(l=i-1;l<=0;l--)
									  {
							    		  if(Character.getNumericValue(ph[i][l])==team)
							    		  {
							    			  if(north>=l)
							    			  {
							    				  north=l;
							    			  } 
							    			  blocknums++;
							    			  ph[i][l]=' ';
										  } 
							          }
					              }
							  } 
				          }
				      }
	                  //Check south
				      if(i + 1 < photo.length)
				      {
				    	  for(k=i+1;k<photo.length;k++)
						  {
				    		  if(Character.getNumericValue(ph[i][k])==team)
				    		  {
				    			  if(south<=k)
				    			  {
				    				  south=k;
				    			  }
				    			  blocknums++;
				    			  ph[i][k]=' ';
				    			  //check east
								  if(j + 1 < photo[i].length())
							      {
									  for(l=j+1;l<photo[i].length();l++)
									  {
										  if(Character.getNumericValue(ph[i][l])==team)
										  {
											  if(east<=l)
											  {
												  east=l;
											  } 
											  blocknums++;
											  ph[i][l]=' ';
										  }  
									  }    
							      }
							      //Check west
							      if(j-1 >= 0)
							      {
							    	  for(l=j-1;l<=0;l--)
									  {
							    		  if(Character.getNumericValue(ph[i][l])==team)
							    		  {
							    			  if(west>=l)
							    			  {
							    				  west=l; 
							    			  }
							    			  blocknums++;
							    			  ph[i][l]=' ';
										  } 
							          }
							      }
				                  //Check south
							      if(i + 1 < photo.length)
							      {
							    	  for(l=i+1;l<photo.length;l++)
									  {
							    		  if(Character.getNumericValue(ph[i][l])==team)
							    		  {
							    			  if(south<=l)
							    			  {
							    				  south=l;
							    			  }
							    			  blocknums++;
							    			  ph[i][l]=' ';
										  } 
							          }
							      }
							      //Check north
							      if(i - 1 >= 0)
							      {
							    	  for(l=i-1;l<=0;l--)
									  {
							    		  if(Character.getNumericValue(ph[i][l])==team)
							    		  {
							    			  if(north>=l)
							    			  {
							    				  north=l;
							    			  } 
							    			  blocknums++;
							    			  ph[i][l]=' ';
										  } 
							          }
					              }
							  } 
				          }
				      }
				      //Check north
				      if(i - 1 >= 0)
				      {
				    	  for(k=i-1;k<=0;k--)
						  {
				    		  if(Character.getNumericValue(ph[i][k])==team)
				    		  {
				    			  if(north>=k)
				    			  {
				    				  north=k;
				    			  } 
				    			  blocknums++;
				    			  //check east
								  if(j + 1 < photo[i].length())
							      {
									  for(l=j+1;l<photo[i].length();l++)
									  {
										  if(Character.getNumericValue(ph[i][l])==team)
										  {
											  if(east<=l)
											  {
												  east=l;
											  } 
											  blocknums++;
											  ph[i][l]=' ';
										  }  
									  }    
							      }
							      //Check west
							      if(j-1 >= 0)
							      {
							    	  for(l=j-1;l<=0;l--)
									  {
							    		  if(Character.getNumericValue(ph[i][l])==team)
							    		  {
							    			  if(west>=l)
							    			  {
							    				  west=l; 
							    			  }
							    			  blocknums++;
							    			  ph[i][l]=' ';
										  } 
							          }
							      }
				                  //Check south
							      if(i + 1 < photo.length)
							      {
							    	  for(l=i+1;l<photo.length;l++)
									  {
							    		  if(Character.getNumericValue(ph[i][l])==team)
							    		  {
							    			  if(south<=l)
							    			  {
							    				  south=l;
							    			  }
							    			  blocknums++;
							    			  ph[i][l]=' ';
										  } 
							          }
							      }
							      //Check north
							      if(i - 1 >= 0)
							      {
							    	  for(l=i-1;l<=0;l--)
									  {
							    		  if(Character.getNumericValue(ph[i][l])==team)
							    		  {
							    			  if(north>=l)
							    			  {
							    				  north=l;
							    			  } 
							    			  blocknums++;
							    			  ph[i][l]=' ';
										  } 
							          }
					              }
							  } 
				          }
		              }
				      int x=east+west+1;
				      int y=north+south+1;
				      if(blocknums>=minblock)
				      {
				    	  result[count]=new Point(x,y);
				    	  count++;
				      }
					 } 
		            }
		        }
			i=0;
			int size=0;
			while(result[i]!=null)
			{
				size++;
				i++;
			}	
	  
			return result;
		}
}    
