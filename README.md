Программа 1: 

namespace WindowsFormsApp2
{
    public partial class Form1 : Form
    {
        public Form1()
        {
            InitializeComponent();
        }

        private void button1_Click(object sender, EventArgs e)
        {
            double a = 0, b = 0, c = 0, d = 0, abstand=0;
            a = Convert.ToDouble(textBox1.Text);
            b = Convert.ToDouble(textBox2.Text);
            c = Convert.ToDouble(textBox3.Text);
            d = Convert.ToDouble(textBox4.Text);
            abstand = Math.Sqrt(Math.Pow((c - a), 2) + Math.Pow((d - b), 2));
            textBox5.Text = Convert.ToString(abstand);
        }

        private void button2_Click(object sender, EventArgs e)
        {
            textBox1.Text = ""; textBox2.Text = ""; textBox3.Text = ""; textBox4.Text = ""; textBox5.Text = "";
        }
    }
}
Программа 2: 
namespace WindowsFormsApp2
{
    public partial class Form1 : Form
    {
        public Form1()
        {
            InitializeComponent();
        }

        private void button1_Click(object sender, EventArgs e)
        {
            double a = 0;
            a = Convert.ToDouble(textBox4.Text);
            if (a % 2 == 1)
            {
                MessageBox.Show("Число нечётное");
            }
            else
            {
                MessageBox.Show("Число чётное");
            }
        }

        private void button2_Click(object sender, EventArgs e)
        {
            textBox4.Text = ""; 
        }
    }
}

