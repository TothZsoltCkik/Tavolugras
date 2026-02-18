# Tavolugras
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Tavolugras
{
    internal class Student
    {
        private string name;
        private string city;
        private List<int> results = new List<int>();

        public Student(string name, string city, string result)
        {
            this.name = name;
            this.city = city;
            foreach (var item in result.Split(' '))
            {
                results.Add(int.Parse(item));   
            }
        }

        public override string ToString()
        {
            return $"{name} ({city})";
        }


    }
}
