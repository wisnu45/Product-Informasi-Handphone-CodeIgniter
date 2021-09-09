# Product-Informasi-Handphone-CodeIgniter

**URL Menuju Admin 
http://localhost/Product_Info/superadmin/**

CODE:
public function login_superadmin($data)
    {
        $login = $this->db->get_where('superadmin', $data);
        if($login->row())
        {
            return $login->row();
        }
        else
        {
            return false;
        }
    }
    
    ![image](https://user-images.githubusercontent.com/45603735/132663684-6061db86-130b-47e6-9502-eced6bd16dde.png)


**URL Menuju Home
http://localhost/Product_Info/**

CODE:
 public function view_item($id)
    {
        $products = $this->db->get_where('products', array('id' => $id));
        return $products->row();
    }
    
    

