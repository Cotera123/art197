
            dataGridView1.DataSource = абонентBindingSource;
            dataGridView1.Columns["Льготы"].Visible = false;
            dataGridView1.Columns["Субсидии"].Visible = false;
            dataGridView1.Columns["Дата регистрации"].Visible = false;
            dataGridView1.Columns["Код адреса"].Visible = false;


            if (dataGridView1.DataSource == абонентBindingSource)
            {
                адресBindingSource.Filter = String.Format("CONVERT(Улица, 'System.String') LIKE '{0}'", АдресTextBox.Text);
            }
            else 
            { MessageBox.Show("ytnvfhg"); }
           
