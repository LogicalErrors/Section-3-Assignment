# Section-3-Assignment
Section 3 Assignment code

using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace Section3Project
{
    public partial class frmStatistics : Form
    {
        public frmStatistics()
        {
            InitializeComponent();
        }

        private void lblResults_Click(object sender, EventArgs e)
        {

        }

        private void btnClear_Click(object sender, EventArgs e)
        {
            textBox1.Text = "";
        }

        private void btnStatus_Click(object sender, EventArgs e)
        {
            string inputString = Console.ReadLine();
            string[] results = inputString.Split(new char[] { ',', ' ', '.' });
            int countOfWords = 0;
            for(int i=0; i<results.Length; i++)
            {
                Console.WriteLine($"{results[i]}");
                countOfWords++;
            }
            Console.WriteLine($"Number of words; {countOfWords}");

        }

        private void btnExit_Click(object sender, EventArgs e)
        {
            this.Close();
        }

        private void txtBoxSentences_TextChanged(object sender, EventArgs e)
        {

        }
    }
}
