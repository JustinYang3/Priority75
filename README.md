# Task Class
implements Priority{
	  private String myTask;
    private int myPriority;

    public Task (String chore, int level) 
    {
        myTask = chore;
        myPriority = level;
    }

    public void setPriority (int level)
    {
        myPriority = level;
    }

    public int getPriority()
    {
        return myPriority;
    }

    public String getTask()
    {
        return myTask;
    }

    public String toString()
    {
        return ("Task: " + getTask() + "\nPriority: " + getPriority());
    }
}

# main
		    Task task1 = new Task ("Do homework", 1);
        Task task2 = new Task ("Sleep", 2);

        task1.setPriority(2);
        task2.setPriority(1);
        
        System.out.println(task1);
        System.out.println(task2);
        
# interface
public interface Priority {
	  public void setPriority (int priority);
    public int getPriority();
}
