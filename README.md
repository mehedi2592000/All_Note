    Linq Code

    ==> Sorting
      1. OrderBY
      2. OrderByDesending
      3. ThenBY  -- you want to sort second row in same time orderby(x=>x.FirstName).ThenBy(y=>y.SecondNAme).TOLIst();
      4. ThenByDesending
      5. Reverse
    ==>QUantifier OPeration 
        1. All
        2. ANy 
        3. Contains
    ==
    ==Set Operation
        1. Distinct == same value have multiple time but you want every value one time 
        2. except == a table b table , a data show which are not match b table data 
        3. interset == a table common data show which is matcher b table
        4. union == show all data
    Partition Methode
        1. Take   == show how many data you want to pick
        2. TakeWhile
        3. skip  == which data you want to skip and show rest one data 
        4. skipWhile

        
    Join Methode
    
         Inner JOin::
            var innerJoin=from student in studets
        		join address in address
        		on student.AddessId equals address.Id
        		select new
        		{
        			studentname=student.Name,
        			studentAddrss=address.Address
        		}.ToList();
            =========================================================
         Inner JOin: Multiple Table:
            
            var innerJoin=from student in studets
            		join address in address
            		on student.AddessId equals address.Id
            		join marks in Marks
            		on student.Id equals marks.Id 
            		select new
            		{
            			studentname=student.Name,
            			studentAddrss=address.Address,
            			studentMarks=a
            		}.ToList();
            =========================================================
         Left Join 
            
            var leftJoinQuery =
                from leftItem in leftCollection
                join rightItem in rightCollection
                on leftItem.Key equals rightItem.Key into joinedItems
                from resultItem in joinedItems.DefaultIfEmpty()
                select new
                {
                    LeftValue = leftItem.Value,
                    RightValue = (resultItem != null) ? resultItem.Value : null // Handle null values
                };
            =============
            
         Right Join
            
            var rightJoinQuery =
                from rightItem in rightCollection
                join leftItem in leftCollection
                on rightItem.Key equals leftItem.Key into joinedItems
                from resultItem in joinedItems.DefaultIfEmpty()
                select new
                {
                    RightValue = rightItem.Value,
                    LeftValue = (resultItem != null) ? resultItem.Value : null // Handle null values
                };

        
