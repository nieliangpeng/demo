# demo



package lww.class16;

import java.io.File;
import java.io.FileReader;
import java.io.FileWriter;
import java.io.IOException;

public class FileTest {

	public static void main(String[] args) {
		
		File file = new File("D://lww");
		if(!file.exists()){
			file.mkdir();
			System.out.println("文件夹创建成功");
		}else{

			
			String[] files = file.list();
			for(int i = 0; i < files.length; i++){
				System.out.println(files[i]);
			}
		}
		
		
		File fileDrectory = new File("D://lww//test.txt");
		if(!fileDrectory.exists()){
			
			try {
				fileDrectory.createNewFile();
				
				FileWriter writer = new FileWriter(fileDrectory);
				writer.write("Hello,lww");
				writer.close();
				System.out.println("写入文件成功");
				FileReader reader = new FileReader(fileDrectory);
				char[] chs = new char[20];
				System.out.println(reader.read(chs));
				reader.close();
			} catch (IOException e) {
				System.out.println("文件创建失败，无法写入信息");
				e.printStackTrace();
			}
			
		} else {

		}
	}

}

