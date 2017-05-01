# demo

demo to github

package lww.class16;

import java.io.File;
import java.io.FileReader;
import java.io.FileWriter;
import java.io.IOException;

public class FileTest {

	public static void main(String[] args) {
		//目录操作
		File file = new File("D://lww");
		if(!file.exists()){//判断存在性
			file.mkdir();//创建目录
			System.out.println("文件夹创建成功");
		}else{
//			System.out.println("文件夹已经存在");
//			file.delete();
//			System.out.println("文件夹已经被删除");
			//文件夹存在，打印文件夹中的文件
			String[] files = file.list();
			for(int i = 0; i < files.length; i++){
				System.out.println(files[i]);
			}
		}
		
		//文件操作
		File fileDrectory = new File("D://lww//test.txt");
		if(!fileDrectory.exists()){
			//不存在，则创建
			try {
				fileDrectory.createNewFile();
				//向文件中写入信息
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
			//文件存在，删除
//			fileDrectory.delete();
//			System.out.println("文件已删除");
		}
	}

}

