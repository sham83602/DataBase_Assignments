# summary report 
select count(*), min(sal), max(Sal), sum(Sal) , avg(sal) from emp;

# matrix report 
select count(*), min(Sal), max(Sal), sum(Sal) from emp group by deptno, order by 1;

select max(sum_Sal) from(select sum(sal) sum_Sal from emp group by deptno) as abcd;

# 2nd largest 

select max(sal) from emp 
where sal <(select max(sal) from emp);
