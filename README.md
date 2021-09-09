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
    



**URL Menuju Home
http://localhost/Product_Info/**

CODE:
 public function view_item($id)
    {
        $products = $this->db->get_where('products', array('id' => $id));
        return $products->row();
    }
    
    

