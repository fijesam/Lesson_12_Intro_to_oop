# Lesson_12_Intro_to_oop
// Exercise 1
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Lesson_11_OOP
{
    public class school
    {
        string _name;
        public school()
        {
            _name = "KST";
        }

        public school(string name)
        {
            _name = name;
        }

        public void teacher()
        {
            Console.Write("Enter the number of teachers: ");
            int x = int.Parse(Console.ReadLine());
            string[] array = new string[x];
            for (int i = 0; i < x; i++)
            {
                // Enter teacher's name below
                Console.Write("array{0} = ", i);
                array[i] = Console.ReadLine();
            }
            Console.WriteLine(array);
   
        }
        public void course()
        {
            Console.WriteLine();
        }


        public string classList
        {
            get { return classList; }
            set { classList = value; }
        }
        public string teachers
        {
            get { return teachers; }
            set { teachers = value; }
        }

        public string courses
        {
            get { return courses; }
            set { courses = value; }
        }
        
    }
}

//Exercise 2
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Lesson_11_OOP
{
    public abstract class Human
    {
        public Human()
        {
            Console.WriteLine("I am Human");
        }
        
        public string firstname
        {
            get { return firstname; }
            set { firstname = value; }
        }

        public string lastname
        {
            get { return lastname; }
            set { lastname = value; }
        }
    }

    public class Student : Human 
    {
        public Student()
        {

        }
        

        public int Mark
        {
            get { return Mark; }
            set { Mark = value; }
        }

    }
    public class Worker: Human
    {
        public Worker()
        {

        }
        public int hourlywage()
        {
            return hour * wage;
        }
        public int hour
        {
            get { return hour; }
            set { hour = value; }
        }
        public int wage
        {
            get { return wage; }
            set { wage = value; }
        }
    }
}

//Exercise 5
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Lesson_11_OOP
{
    public abstract class Shape
    {
        public Shape()
        {

        }
        public abstract int CalculateSurface();

        private int width;
        private int height;

    }
    public class Rectangle : Shape
    {
        public override int CalculateSurface()
        {
            throw new NotImplementedException();
        }
    }
    public class Triangle : Shape
    {
        public override int CalculateSurface()
        {
            throw new NotImplementedException();
        }

    }

    public class Circle : Shape
    {
        public Circle(int width, int height)
        {

        }

     
        public override int CalculateSurface()
        {
            throw new NotImplementedException();
        }

        private int radius;
    }
}

//Exercise 6
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Lesson_11_OOP
{
    public abstract class Animal
    {
        public Animal()
        {

        }

        public virtual void Sound()
        {
            return;
        }

        public int name { get; set; }
        public int age { get; set; }
        public int gender { get; set; }
    }
    public class Dog : Animal
    {

    }
    public class Frog : Animal
    {

    }
    public class Cat : Animal
    {

    }

    public class Kitten : Animal
    {

    }
    public class Tomcat : Animal
    {

    }
}

