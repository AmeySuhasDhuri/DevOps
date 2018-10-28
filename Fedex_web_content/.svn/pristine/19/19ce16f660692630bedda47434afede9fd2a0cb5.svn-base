package com.fedex.services;

import com.fedex.vo.LoginVo;

public class LoginService {

	public boolean checkLogin(final LoginVo loginVo){
		if(!(loginVo == null)){
			if(!(loginVo.getId() == null)){
				return loginVo.getId().equals(loginVo.getPassword());
			} return false;
		}
		return false;
	}
	
	public static void main(String[] args) {
		/*System.out.println("Result ::: "+checkLogin(new LoginVo("Niteesh", "123")));
		System.out.println("Result ::: "+checkLogin(new LoginVo("123", "123")));
		System.out.println("Result ::: "+checkLogin(new LoginVo("Niteesh", "Niteesh")));
		System.out.println("Result ::: "+checkLogin(null));
		System.out.println("Result ::: "+checkLogin(new LoginVo(null, "123")));
		System.out.println("Result ::: "+checkLogin(new LoginVo(null, null)));
		System.out.println("Result ::: "+checkLogin(new LoginVo("123", null)));*/
	}
	
	
}
